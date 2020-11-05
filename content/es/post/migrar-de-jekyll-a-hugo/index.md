---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Migrar De Jekyll a Hugo"
subtitle: ""
summary: "Jekyll tiene una regla de que cualquier directorio que no comience con `_` se copiará tal cual a la salida `_site`. Hugo mantiene todo el contenido estático bajo 'static'. Por lo tanto, debe moverlo todo allí. Con Jekyll, algo que parecía..."
authors: []
tags: [
  Hugo,
  Jekyll,
]
categories: [
  Tecnologías,
  Tutoriales,
]
date: 2020-01-19
lastmod: 2020-01-19
featured: true
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  placement: 1
  caption: 'Image credit: [**Github**](https://github.com/)'
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
# projects: []
---

## Mover contenido estático a `static`
Jekyll tiene una regla de que cualquier directorio que no comience con `_` se copiará tal cual a la salida `_site`. Hugo mantiene todo el contenido estático bajo 'static'. Por lo tanto, debe moverlo todo allí.
Con Jekyll, algo que parecía

    ▾ <root>/
        ▾ images/
            logo.png

en Hugo debería ser

    ▾ <root>/
        ▾ static/
            ▾ images/
                logo.png

Además, querrá que los archivos que deberían residir en la raíz (como `CNAME`) se muevan a `static`.

## Crea tu archivo de configuración de Hugo
Hugo puede leer su configuración como JSON, YAML o TOML. Hugo también admite parámetros de configuración personalizada. Consulte la [documentación de configuración de Hugo](/overview/configuration/) para obtener más detalles.

## Establezca su carpeta de publicación de configuración en `_site`
El valor predeterminado es que Jekyll publique en `_site` y que Hugo publique en `public`. Si, como yo, tiene [`_site` asignado a un submódulo git en la rama `gh-pages`](http://blog.blindgaenger.net/generate_github_pages_in_a_submodule.html), querrá hacer una de estas dos alternativas:

1. Cambie su submódulo para apuntar el mapeo de `gh-pages` a `public` en lugar de a `_site` (recomendado).

        git submodule deinit _site
        git rm _site
        git submodule add -b gh-pages git@github.com:your-username/your-repo.git public

2. O cambie la configuración de Hugo para usar `_site` en lugar de `public`.

        {
            ..
            "publishdir": "_site",
            ..
        }

## Convertir plantillas Jekyll a plantillas Hugo
Esa es la mayor parte del trabajo aquí. La documentación es tu amiga. Debes consultar la [documentación de la plantilla de Jekyll](http://jekyllrb.com/docs/templates/) si necesitas actualizar tu memoria sobre cómo construiste tu blog y [la plantilla de Hugo](/layout/templates/) para aprender El modo de Hugo.

Como un solo punto de referencia, la conversión de mis plantillas para [heyitsalex.net](http://heyitsalex.net/) no me llevó más de unas pocas horas.

## Convierte los plugins de Jekyll en shortcodes de Hugo
Jekyll tiene [complementos](http://jekyllrb.com/docs/plugins/); Hugo tiene [códigos cortos](/doc/shortcodes/). Es bastante trivial hacer un port.

### Implementación
Como ejemplo, estaba usando un plugin personalizado [`image_tag`](https://github.com/alexandre-normand/alexandre-normand/blob/74bb12036a71334fdb7dba84e073382fc06908ec/_plugins/image_tag.rb) para generar figuras con subtítulos cuando se ejecuta Jekill. Mientras leía acerca de los shortcodes, descubrí que Hugo tenía un shortcode incorporado que hace exactamente lo mismo.

Complemento de Jekyll:

    module Jekyll
      class ImageTag < Liquid::Tag
        @url = nil
        @caption = nil
        @class = nil
        @link = nil
        // Patterns
        IMAGE_URL_WITH_CLASS_AND_CAPTION =
        IMAGE_URL_WITH_CLASS_AND_CAPTION_AND_LINK = /(\w+)(\s+)((https?:\/\/|\/)(\S+))(\s+)"(.*?)"(\s+)->((https?:\/\/|\/)(\S+))(\s*)/i
        IMAGE_URL_WITH_CAPTION = /((https?:\/\/|\/)(\S+))(\s+)"(.*?)"/i
        IMAGE_URL_WITH_CLASS = /(\w+)(\s+)((https?:\/\/|\/)(\S+))/i
        IMAGE_URL = /((https?:\/\/|\/)(\S+))/i
        def initialize(tag_name, markup, tokens)
          super
          if markup =~ IMAGE_URL_WITH_CLASS_AND_CAPTION_AND_LINK
            @class   = $1
            @url     = $3
            @caption = $7
            @link = $9
          elsif markup =~ IMAGE_URL_WITH_CLASS_AND_CAPTION
            @class   = $1
            @url     = $3
            @caption = $7
          elsif markup =~ IMAGE_URL_WITH_CAPTION
            @url     = $1
            @caption = $5
          elsif markup =~ IMAGE_URL_WITH_CLASS
            @class = $1
            @url   = $3
          elsif markup =~ IMAGE_URL
            @url = $1
          end
        end
        def render(context)
          if @class
            source = "<figure class='#{@class}'>"
          else
            source = "<figure>"
          end
          if @link
            source += "<a href=\"#{@link}\">"
          end
          source += "<img src=\"#{@url}\">"
          if @link
            source += "</a>"
          end
          source += "<figcaption>#{@caption}</figcaption>" if @caption
          source += "</figure>"
          source
        end
      end
    end
    Liquid::Template.register_tag('image', Jekyll::ImageTag)

está escrito como este shortcode de Hugo:

    <!-- image -->
    <figure {{ with .Get "class" }}class="{{.}}"{{ end }}>
        {{ with .Get "link"}}<a href="{{.}}">{{ end }}
            <img src="{{ .Get "src" }}" {{ if or (.Get "alt") (.Get "caption") }}alt="{{ with .Get "alt"}}{{.}}{{else}}{{ .Get "caption" }}{{ end }}"{{ end }} />
        {{ if .Get "link"}}</a>{{ end }}
        {{ if or (or (.Get "title") (.Get "caption")) (.Get "attr")}}
        <figcaption>{{ if isset .Params "title" }}
            {{ .Get "title" }}{{ end }}
            {{ if or (.Get "caption") (.Get "attr")}}<p>
            {{ .Get "caption" }}
            {{ with .Get "attrlink"}}<a href="{{.}}"> {{ end }}
                {{ .Get "attr" }}
            {{ if .Get "attrlink"}}</a> {{ end }}
            </p> {{ end }}
        </figcaption>
        {{ end }}
    </figure>
    <!-- image -->

### Uso
Simplemente cambié:

    {% image full http://farm5.staticflickr.com/4136/4829260124_57712e570a_o_d.jpg "Una de mis fotos favoritas de tipo turístico. Esperé secretamente la buena luz mientras nos estábamos "divirtiendo" y tomé esto. Solo lamento: un estúpido poste en la esquina superior izquierda del marco del que tuve que deshacerme torpemente después del procesamiento." ->http://www.flickr.com/photos/alexnormand/4829260124/in/set-72157624547713078/ %}

por esto (este ejemplo usa una versión ligeramente extendida llamada `fig`, diferente a la `figure` incorporada):

    {{%/* fig class="full" src="http://farm5.staticflickr.com/4136/4829260124_57712e570a_o_d.jpg" title="Una de mis fotos favoritas de tipo turístico. Esperé secretamente la buena luz mientras nos estábamos "divirtiendo" y tomé esto. Solo lamento: un estúpido poste en la esquina superior izquierda del marco del que tuve que deshacerme torpemente después del procesamiento." link="http://www.flickr.com/photos/alexnormand/4829260124/in/set-72157624547713078/" */%}}

Como beneficio adicional, los parámetros de shortcode son, posiblemente, más legibles.

## Últimos retoques
### Reparar contenido
Dependiendo de la cantidad de personalización que se realizó con cada publicación con Jekyll, este paso requerirá más o menos esfuerzo. Aquí no hay reglas estrictas y rápidas, excepto que `hugo server --watch` es tu amigo. Pruebe sus cambios y corrija los errores según sea necesario.

### Limpiar
Querrá eliminar la configuración de Jekyll en este punto. Si tiene algo más que no se usa, elimínelo.

## Un ejemplo práctico en un diff

El sitio [Hola, soy Alex](http://heyitsalex.net/) fue migrado en menos de un día de padre con hijos de Jekyll a Hugo. Puede ver todos los cambios (y atornillamientos) mirando este [diff](https://github.com/alexandre-normand/alexandre-normand/compare/869d69435bd2665c3fbf5b5c78d4c22759d7613a...b7f6605b1265e83b4b81495423294108).
