---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Fundamentos de las plantillas Hugo"
subtitle: ""
summary: "Hugo usa la excelente librería go html/template para su motor de plantillas. Es un extremadamente ligero motor que proporciona una muy pequeña cantidad de lógica."
authors: []
tags: [
  Hugo,
  Go,
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
  caption: 'Image credit: [**Golang**](https://golang.org/)'
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

Hugo usa la excelente librería [go][] [html/template][gohtmltemplate] para su motor de plantillas. Es un motor extremadamente ligero que proporciona una muy pequeña cantidad de lógica. En nuestra experiencia, es la lógica justa para poder crear un buen sitio web estático. Si has utilizado otros sistemas de plantillas de diferentes idiomas o marcos, encontrarás muchas similitudes en las plantillas go.

Este documento es una breve introducción sobre el uso de plantillas go. La [go docs][gohtmltemplate] proporciona más detalles.

## Introducción a las plantillas Go

Las plantillas Go proporcionan un lenguaje de plantillas extremadamente simple. Se adhiere a la creencia de que solo la lógica más básica pertenece a la plantilla o capa de vista. Una consecuencia de esta simplicidad es que las plantillas van a analizar muy rápidamente.

Una característica única de las plantillas go es que son conscientes del contenido. Las variables y el contenido se desinfectarán según el contexto de dónde se usen. Más detalles se pueden encontrar en el [go docs][gohtmltemplate].

## Sintaxis básica

Las plantillas Go Lang son archivos html con la adición de variables y funciones.

**Las variables y funciones Go son accesibles dentro de {{ }}**

Acceder a una variable predefinida "foo":

    {{ foo }}

**Los parámetros se separan usando espacios**

Llamar a la función de agregar con la entrada de 1, 2:

    {{ add 1 2 }}

**Se accede a los métodos y campos a través de la notación de puntos**

Acceder al parámetro de página "bar"

    {{ .Params.bar }}

**Los paréntesis se pueden usar para agrupar elementos**

    {{ if or (isset .Params "alt") (isset .Params "caption") }} Caption {{ end }}


## Variables

Cada plantilla Go tiene una estructura (objeto) disponible. En Hugo, a cada plantilla se le pasa una estructura de página o de nodo, según el tipo de página que esté representando. Más detalles están disponibles en la página [variables](/layout/variables).

Se accede a una variable haciendo referencia al nombre de la variable.

    <title>{{ .Title }}</title>

Las variables también se pueden definir y referenciar.

    {{ $address := "123 Main St."}}
    {{ $address }}


## Funciones

Las plantillas Go vienen con algunas funciones que proporcionan funcionalidad básica. El sistema de plantillas Go también proporciona un mecanismo para que las aplicaciones amplíen las funciones disponibles con las suyas. [Las funciones de la plantilla de Hugo] (/layout/functions) proporcionan algunas funciones adicionales que creemos son útiles para crear sitios web. Las funciones se invocan usando su nombre seguido de los parámetros requeridos separados por espacios. Las funciones de plantilla no se pueden agregar sin recompilar hugo.

**Ejemplo:**

    {{ add 1 2 }}

## Inclusiones

Al incluir otra plantilla, le pasará los datos que serán
accesibles. Para transmitir el contexto actual, recuerde
incluir un punto final. La ubicación de las plantillas siempre comenzará en el directorio /layout/ dentro de Hugo.

**Ejemplo:**

    {{ template "chrome/header.html" . }}


## Lógica

Las plantillas Go proporcionan la iteración más básica y la lógica condicional.

### Iteración

Al igual que en Go, las plantillas Go hacen un uso intensivo del rango para iterar sobre un mapa, matriz o corte. Los siguientes son diferentes ejemplos de cómo usar el rango.

**Ejemplo 1: Usando contexto**

    {{ range array }}
        {{ . }}
    {{ end }}

**Ejemplo 2: Declarando valor nombre de variable**

    {{range $element := array}}
        {{ $element }}
    {{ end }}

**Ejemplo 3: Declaración de nombre de variable de clave y valor**

    {{range $index, $element := array}}
        {{ $index }}
        {{ $element }}
    {{ end }}

### Condicionales

If, else, with, or, & and, proporcionan el marco para el manejo de la lógica condicional en las plantillas Go. Al igual que el rango, cada declaración se cierra con `end`.

Las plantillas Go tratan los siguientes valores como falsos:

* false
* 0
* cualquier array, slice, map o string de longitud cero

**Ejemplo 1: If**

    {{ if isset .Params "title" }}<h4>{{ index .Params "title" }}</h4>{{ end }}

**Ejemplo 2: If -> Else**

    {{ if isset .Params "alt" }}
        {{ index .Params "alt" }}
    {{else}}
        {{ index .Params "caption" }}
    {{ end }}

**Ejemplo 3: And & Or**

    {{ if and (or (isset .Params "title") (isset .Params "caption")) (isset .Params "attr")}}

**Ejemplo 4: With**

Una forma alternativa de escribir "if" y luego hacer referencia al mismo valor es usar "with" en su lugar. With vuelve a unir el contexto `.` dentro de su alcance,
y omite el bloque si la variable está ausente.

El primer ejemplo anterior podría simplificarse como:

    {{ with .Params.title }}<h4>{{ . }}</h4>{{ end }}

**Ejemplo 5: If -> Else If**

    {{ if isset .Params "alt" }}
        {{ index .Params "alt" }}
    {{ else if isset .Params "caption" }}
        {{ index .Params "caption" }}
    {{ end }}

## Tuberías

Uno de los componentes más poderosos de las plantillas Go es la capacidad de apilar acciones una tras otra. Esto se hace mediante el uso de tuberías. Tomado de tuberías Unix, el concepto es simple, la salida de cada tubería se convierte en la entrada de la siguiente tubería.

Debido a la sintaxis muy simple de las plantillas Go, la tubería es esencial para poder encadenar llamadas de función. Una limitación de las tuberías es que solo pueden funcionar con un único valor y ese valor se convierte en el último parámetro de la siguiente tubería.

Algunos ejemplos simples deberían ayudar a cómo usar la tubería.

**Ejemplo 1 :**

    {{ if eq 1 1 }} Same {{ end }}

es lo mismo que

    {{ eq 1 1 | if }} Same {{ end }}

Parece extraño colocar el if al final, pero proporciona una buena ilustración de cómo usar las tuberías.

**Ejemplo 2 :**

    {{ index .Params "disqus_url" | html }}

Accede al parámetro de página llamado "disqus_url" y escapa el HTML.

**Ejemplo 3 :**

    {{ if or (or (isset .Params "title") (isset .Params "caption")) (isset .Params "attr")}}
    Cosas aquí
    {{ end }}

Podría ser reescrito como

    {{  isset .Params "caption" | or isset .Params "title" | or isset .Params "attr" | if }}
    Stuff Here
    {{ end }}


## Contexto (también conocido como el punto)

El concepto más fácil de pasar por alto para entender sobre las plantillas Go es que {{ . }} siempre se refiere al contexto actual. En el nivel superior de su plantilla, este será el conjunto de datos disponible. Dentro de una iteración tendrá el valor del elemento actual. Cuando está dentro de un bucle, el contexto ha cambiado.. ya no se referirá a los datos disponibles para toda la página. Si necesita acceder a esto desde el bucle, es probable que desee establecerlo en una variable en lugar de depender del contexto.

**Ejemplo:**

      {{ $title := .Site.Title }}
      {{ range .Params.tags }}
        <li> <a href="{{ $baseurl }}/tags/{{ . | urlize }}">{{ . }}</a> - {{ $title }} </li>
      {{ end }}

Observe cómo una vez que hemos ingresado al bucle, el valor de {{ . }} ha cambiado. Hemos definido una variable fuera del ciclo para tener acceso a ella desde dentro del ciclo.

# Parámetros de Hugo

Hugo ofrece la opción de pasar valores al lenguaje de plantilla a través de la configuración del sitio (para valores de todo el sitio), o a través del metadatos de cada pieza específica de contenido. Puede definir cualquier valor de cualquier tipo (compatible con su formato FrontMatter/config) y usarlo dentro de sus plantillas.


## Uso de parámetros de contenido (página)

En cada pieza de contenido, puede proporcionar variables para ser utilizadas por plantillas. Esto sucede en el [front matter](/content/front-matter).

Un ejemplo de esto se utiliza en este sitio de documentación. La mayoría de las páginas se benefician de tener la tabla de contenido proporcionada. A veces, el TOC simplemente no tiene mucho sentido. Hemos definido una variable en el frente de algunas páginas para desactivar la visualización de la tabla de contenido.

Aquí está el ejemplo de front matter:

```
---
title: "Permalinks"
date: "2013-11-18"
aliases:
  - "/doc/permalinks/"
groups: ["extras"]
groups_weight: 30
notoc: true
---
```

Aquí está el código correspondiente dentro de la plantilla:

      {{ if not .Params.notoc }}
        <div id="toc" class="well col-md-4 col-sm-6">
        {{ .TableOfContents }}
        </div>
      {{ end }}



## Uso de los parámetros del sitio (config)

En su archivo de configuración de nivel superior (Ej. `config.yaml`) puede definir los parámetros del sitio, que son valores que estarán disponibles en Chrome.

Por ejemplo, puede declarar:

```
params:
  CopyrightHTML: "Copyright &#xA9; 2013 John Doe. All Rights Reserved."
  TwitterUser: "spf13"
  SidebarRecentLimit: 5
```

Dentro de un layout de pie de página, puede declarar un `<footer>` que solo se proporciona si se recibe el parámetro `CopyrightHTML`, y si se proporciona, debería declarar que es HTML-safe, de modo que la entidad HTML no escapé de nuevo. Esto permitirá actualizar fácilmente sólo el archivo de configuración de nivel superior cada 1 de enero, en lugar de la caza a través de sus plantillas.

```
{{if .Site.Params.CopyrightHTML}}<footer>
<div class="text-center">{{.Site.Params.CopyrightHTML | safeHtml}}</div>
</footer>{{end}}
```

Una forma alternativa de escribir el "if" y luego hacer referencia al mismo valor es usar "with" en su lugar. With vuelve a unir el contexto `.` dentro de su alcance y omite el bloque si la variable está ausente:

```
{{with .Site.Params.TwitterUser}}<span class="twitter">
<a href="https://twitter.com/{{.}}" rel="author">
<img src="/images/twitter.png" width="48" height="48" title="Twitter: {{.}}"
 alt="Twitter"></a>
</span>{{end}}
```

Finalmente, si desea extraer "constantes mágicas" de sus diseños, puede hacerlo, como en este ejemplo:

```
<nav class="recent">
  <h1>Posts recientes</h1>
  <ul>{{range first .Site.Params.SidebarRecentLimit .Site.Recent}}
    <li><a href="{{.RelPermalink}}">{{.Title}}</a></li>
  {{end}}</ul>
</nav>
```


[go]: <http://golang.org/>
[gohtmltemplate]: <http://golang.org/pkg/html/template/>
