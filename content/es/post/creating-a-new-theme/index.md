---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Crear un tema simple en Hugo"
subtitle: ""
summary: "Este tutorial te mostrará cómo crear un tema simple en Hugo. Supongo que estás familiarizado con HTML, la línea de comando bash, y que te sientes cómodo usando Markdown para formatear contenido. Explicaré cómo Hugo usa plantillas y cómo puedes organizar tus plantillas para crear un tema. No cubriré el uso de CSS para diseñar el tema."
authors: []
tags: [
  Hugo,
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
  caption: 'Image credit: [**Halogenica**](https://github.com/halogenica)'
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
# projects: []
---


## Introducción

Este tutorial te mostrará cómo crear un tema simple en Hugo. Supongo que estás familiarizado con HTML, la línea de comando bash, y que te sientes cómodo usando Markdown para formatear contenido. Explicaré cómo Hugo usa plantillas y cómo puedes organizar tus plantillas para crear un tema. No cubriré el uso de CSS para diseñar el tema.

Comenzaremos creando un nuevo sitio con una plantilla muy básica. Luego agregaremos algunas páginas y publicaciones. Con pequeñas variaciones al respecto, podrás crear muchos tipos diferentes de sitios web.

En este tutorial, los comandos que ingrese comenzarán con "$", a lo que seguirá la salida. Las líneas que comienzan con "#" son comentarios que he agregado para explicar un punto. Cuando muestro actualizaciones a un archivo, el ": wq" en la última línea significa guardar el archivo.

Aquí va un ejemplo:

{{< gist naujoel 9813fc841c7ff14f57dd224bce4c708d >}}

## Algunas definiciones

Hay unos pocos conceptos que necesitas comprender antes de crear un tema.

### Skins (Máscaras)

Las máscaras son los archivos responsables de la apariencia de tu sitio. Es el CSS que controla los colores y las fuentes, es el Javascript que determina las acciones y reacciones. También son las reglas que usa Hugo para transformar el contenido en el HTML que el sitio servirá a los visitantes.

Tienes dos formas de crear una máscara. La forma más simple es crearlo en el directorio ```layouts/```. Si lo haces, no tienes que preocuparte por configurar Hugo para que lo reconozca. El primer lugar donde Hugo buscará reglas y archivos es en el directorio ```layouts/``` para que siempre encuentre la máscara.

La segunda opción es crearlo en un subdirectorio del directorio ```themes/```. Si lo haces, siempre debes decirle a Hugo dónde buscar la máscara. Sin embargo, es un trabajo extra, entonces, ¿por qué molestarse con él?

La diferencia entre crear una máscara en ```layouts/``` y crearla en ```themes/``` es muy sutil. Una máscara en ```layouts/``` no se puede personalizar sin actualizar las plantillas y los archivos estáticos a partir de los cuales está construida. Una máscara creada en ```themes/```, por otro lado, puede ser y eso facilita que otras personas la usen.

El resto de este tutorial llamará tema a un skin creado en el directorio ```themes/```.

Ten en cuenta que puedes usar este tutorial para crear una máscara en el directorio ```layouts/``` si lo deseas. La principal diferencia será que no necesitarás actualizar el archivo de configuración del sitio para usar un tema.

### La página de inicio

La página de inicio, o página de destino, es la primera página que ven muchos visitantes de un sitio. Es el archivo index.html en el directorio raíz del sitio web. Como Hugo escribe archivos en el directorio ```public/```, nuestra página de inicio es ```public/index.html```.

### El archivo de configuración del sitio

Cuando se ejecuta Hugo, busca un archivo de configuración que contenga configuraciones que anulen los valores predeterminados para todo el sitio. El archivo puede usar TOML, YAML o JSON. Prefiero usar TOML para mis archivos de configuración. Si prefieres usar JSON o YAML, deberás traducir mis ejemplos. También deberás cambiar el nombre del archivo, ya que Hugo usa la extensión para determinar cómo procesarlo.

Hugo traduce los archivos de Markdown a HTML. Por defecto, Hugo espera encontrar archivos Markdown en tu directorio ```content/``` y archivos de plantilla en su directorio ```themes/```. Hugo creará archivos HTML en su directorio ```public/```. Puedes cambiar esto especificando ubicaciones alternativas en el archivo de configuración.

### Contenido

El contenido se almacena en archivos de texto que contienen dos secciones. La primera sección es la "front matter", que es la metainformación sobre el contenido. La segunda sección contiene Markdown que se convertirá a HTML.

#### Front Matter

La Front Matter es la información sobre el contenido. Al igual que el archivo de configuración, puede escribirse en TOML, YAML o JSON. A diferencia del archivo de configuración, Hugo no usa la extensión del archivo para conocer el formato. Busca marcadores para señalar el tipo. TOML está rodeado por “`+++`”, YAML por “`---`” y JSON está encerrado entre llaves. Prefiero usar TOML, por lo que deberás traducir mis ejemplos si prefiere YAML o JSON.

La información de la Front Matter se pasa a la plantilla antes de que el contenido se procese en HTML.

#### Markdown

El contenido está escrito en Markdown, lo que facilita la creación del contenido. Hugo ejecuta el contenido a través de un motor Markdown para crear el HTML que se escribirá en el archivo de salida.

### Archivos de plantilla

Hugo usa archivos de plantilla para representar el contenido en HTML. Los archivos de plantilla son un puente entre el contenido y la presentación. Las reglas en la plantilla definen qué contenido se publica, dónde se publica y cómo se representará en el archivo HTML. La plantilla guía la presentación especificando el estilo a utilizar.

Hay tres tipos de plantillas: individual, lista y parcial. Cada tipo toma un poco de contenido como entrada y lo transforma en función de los comandos de la plantilla.

Hugo utiliza su conocimiento del contenido para encontrar el archivo de plantilla utilizado para representar el contenido. Si no puede encontrar una plantilla que coincida exactamente con el contenido, cambiará de nivel y buscará desde allí. Continuará haciéndolo hasta que encuentre una plantilla coincidente o se quede sin plantillas para probar. Si no puede encontrar una plantilla, utilizará la plantilla predeterminada para el sitio.

Ten en cuenta que puedes utilizar la Front Matter para influir en la elección de plantillas de Hugo.

#### Plantilla individual

Se utiliza una plantilla individual para representar una sola pieza de contenido. Por ejemplo, un artículo o publicación sería una sola pieza de contenido y usaría una sola plantilla.

#### Plantilla de lista

Una plantilla de lista representa un grupo de contenido relacionado. Eso podría ser un resumen de publicaciones recientes o de todos los artículos de una categoría. Las plantillas de lista pueden contener múltiples grupos.

La plantilla de la página de inicio es un tipo especial de plantilla de lista. Hugo asume que la página de inicio de su sitio actuará como el portal para el resto del contenido del sitio.

#### Plantilla parcial

Una plantilla parcial es una plantilla que se puede incluir en otras plantillas. Las plantillas parciales deben llamarse utilizando el comando de plantilla ```partial```. Son muy útiles para acumular comportamientos comunes. Por ejemplo, tu sitio puede tener un banner que usan todas las páginas. En lugar de copiar el texto del banner en cada plantilla individual y de lista, puedes crear una plantilla parcial con el banner en ella. De esa manera, si decides cambiar el banner, solo tiene que cambiar la plantilla parcial.

## Crear un nuevo sitio

Usemos a Hugo para crear un nuevo sitio web. Soy usuario de Mac, así que crearé el mío en mi directorio de inicio, en la carpeta Sitios. Si estás utilizando Linux, es posible que primero debas crear la carpeta.

El comando ```new site``` creará un esqueleto de un sitio. Le dará la estructura básica del directorio y un archivo de configuración utilizable.

{{< gist naujoel 9e09971dad357c893b4d4fe850fbf1fe >}}

Echa un vistazo en el directorio ```content/``` para confirmar que está vacío.

Los otros directorios (```archetypes/```, ```layouts/```, and ```static/```) se utilizan al personalizar un tema. Ese es un tema para un tutorial diferente, así que ignóralos por ahora.

### Generar el HTML para el nuevo sitio

Ejecutar el comando ```hugo``` sin opciones leerá todo el contenido disponible y generará los archivos HTML. También copiará todos los archivos estáticos (eso es todo lo que no es contenido). Como tenemos un sitio vacío, no servirá de mucho, pero lo hará muy rápidamente.

{{< gist naujoel fce0057406c13a13ce5d27b3818b1ba8 >}}

El indicador ```--verbose``` proporciona información adicional que será útil cuando creemos la plantilla. Cada línea de la salida que comienza con ```INFO:``` o ```WARN:``` está presente porque usamos esa bandera. Las líneas que comienzan con ```WARN:``` son mensajes de advertencia. Los revisaremos más tarde.

Podemos verificar que el comando funcionó mirando el directorio nuevamente.

{{< gist naujoel da85c669816e4fab50c797404f316443 >}}

¿Ves ese nuevo directorio ```public/```? Hugo colocó todo el contenido generado allí. Cuando estés listo para publicar tu sitio web, ese es el lugar para comenzar. Sin embargo, por ahora, confirmemos que tenemos lo que esperaríamos de un sitio sin contenido.

{{< gist naujoel 2827f456bab37fe36754ed9086ad15a2 >}}

Hugo creó dos archivos XML, que es estándar, pero no hay archivos HTML.

### Probar el nuevo sitio

Verifica que puedes ejecutar el servidor web incorporado. Si lo haces, acortarás drásticamente el ciclo de desarrollo. Comienza ejecutando el comando ```server```. Si tienes éxito, verás una salida similar a la siguiente:

{{< gist naujoel ff18df33d4c258dee422d8b34ffb997b >}}

Conéctate a la URL indicada (está en la línea que comienza con ```Web Server```). Si todo funciona correctamente, deberías obtener una página que muestre lo siguiente:

{{< highlight html >}}
index.xml
sitemap.xml
{{< /highlight >}}

Esa es una lista del directorio ```public/```. Hugo no creó una página de inicio porque nuestro sitio no tiene contenido. Cuando no hay un archivo index.html en un directorio, el servidor enumera los archivos en el directorio, que es lo que deberías ver en tu navegador.

Volvamos y miremos esas advertencias nuevamente.

{{< highlight html >}}
WARN: 2014/09/29 Unable to locate layout: [index.html _default/list.html _default/single.html]
WARN: 2014/09/29 Unable to locate layout: [404.html]
{{< /highlight >}}

Esa segunda advertencia es más fácil de explicar. No hemos creado una plantilla para ser utilizada para generar "errores de página no encontrada". El mensaje 404 es un tema para un tutorial por separado.

Ahora para la primera advertencia. Es para la página de inicio. Se nota porque el primer diseño que buscó fue "index.html". Eso solo lo usa la página de inicio.

Me gusta la bandera ```--verbose``` porque hace que Hugo enumere los archivos que está buscando. Para la página de inicio, son index.html, _default/list.html y _default/single.html. Hay algunas reglas que cubriremos más adelante que explican los nombres y las rutas. Por ahora, solo recuerda que Hugo no pudo encontrar una plantilla para la página de inicio y te lo dijo.

En este punto, tienes una instalación y un sitio en funcionamiento sobre los que podemos construir. Todo lo que queda es agregar algo de contenido y un tema para mostrarlo.

## Crear un nuevo tema

Hugo no se envía con un tema predeterminado. Hay algunos disponibles (conté una docena cuando instalé Hugo por primera vez) y Hugo viene con un comando para crear nuevos temas.

Vamos a crear un nuevo tema llamado "zafta". Dado que el objetivo de este tutorial es mostrarte cómo completar los archivos para extraer su contenido, el tema no contendrá ningún CSS. En otras palabras, feo pero funcional.

Todos los temas tienen opiniones sobre el contenido y el diseño. Por ejemplo, Zafta usa "post" sobre "blog". Las opiniones fuertes crean plantillas más simples, pero las opiniones diferentes hacen que sea más difícil usar temas. Cuando crees un tema, considera usar los términos que hacen otros temas.

### Crear un esqueleto

Usa el comando "new" de hugo para crear el esqueleto de un tema. Esto crea la estructura de directorios y coloca archivos vacíos para que los completes.

{{< gist naujoel 163fcfba0d40007a937af5aa9f2739bc >}}

El esqueleto incluye plantillas (los archivos que terminan en .html), el archivo de licencia, una descripción de tu tema (el archivo theme.toml) y un arquetipo vacío.

Tómate un minuto para completar los archivos theme.toml y LICENSE.md. Son opcionales, pero si vas a distribuir tu tema, le dice al mundo a quién alabar (o culpar). También es bueno declarar la licencia para que las personas sepan cómo pueden usar el tema.

{{< gist naujoel 3b1537fc68c90be52ecc2deaf1831aff >}}

Ten en cuenta que los archivos de plantilla del esqueleto están vacíos. No te preocupes, lo cambiaremos en breve.

{{< gist naujoel a60d71a150fd194015fa2561d4f3c5b4 >}}

### Actualiza el archivo de configuración para usar el tema

Ahora que tenemos un tema para trabajar, es una buena idea agregar el nombre del tema al archivo de configuración. Esto es opcional, porque siempre puedes agregar "-t zafta" en todos sus comandos. Me gusta ponerlo en el archivo de configuración porque me gustan las líneas de comando más cortas. Si no lo colocas en el archivo de configuración o no lo especificas en la línea de comando, no utilizarás la plantilla que esperas.

Edita el archivo para agregar el tema, agrega un título para el sitio y especifique que todo nuestro contenido utilizará el formato TOML.

{{< gist naujoel c7b0bacc2f781e5bb81291f9760f92dd >}}

### Generar el sitio

Ahora que tenemos un tema vacío, generemos el sitio nuevamente.

{{< gist naujoel fefaf913ff97a4bc05df54d29b7a0407 >}}

¿Notaste que la salida es diferente? El mensaje de advertencia para la página de inicio ha desaparecido y tenemos una línea de información adicional que dice que Hugo se está sincronizando desde el directorio del tema.

Veamos el directorio ```public/``` para ver qué ha creado Hugo.

{{< gist naujoel bcaf8b0295087dfb07810d8eadbbf2ef >}}

Nota cuatro cosas:

1. Hugo creó una página de inicio. Este es el archivo public/index.html.
2. Hugo creó un directorio css/.
3. Hugo creó un directorio js/.
4. Hugo afirmó que creó 0 páginas. Creó un archivo y lo copió sobre archivos estáticos, pero no creó ninguna página. Esto se debe a que considera que una "página" es un archivo creado directamente a partir de un archivo de contenido. No cuenta cosas como los archivos index.html que crea automáticamente.

#### La página de inicio

Hugo admite muchos tipos diferentes de plantillas. La página de inicio es especial porque obtiene su propio tipo de plantilla y su propio archivo de plantilla. El archivo layouts/index.html se utiliza para generar el HTML para la página de inicio. La documentación de Hugo dice que esta es la única plantilla requerida, pero eso depende. El mensaje de advertencia de Hugo muestra que busca tres plantillas diferentes:

{{< highlight html >}}
WARN: 2014/09/29 Unable to locate layout: [index.html _default/list.html _default/single.html]
{{< /highlight >}}

Si no puede encontrar ninguno de estos, omite completamente la creación de la página de inicio. Notamos eso cuando creamos el sitio sin tener un tema instalado.

Cuando Hugo creó nuestro tema, creó una plantilla de página de inicio vacía. Ahora, cuando construimos el sitio, Hugo encuentra la plantilla y la usa para generar el HTML para la página de inicio. Como el archivo de plantilla está vacío, el archivo HTML también está vacío. Si la plantilla tuviera alguna regla, Hugo la habría usado para generar la página de inicio.

{{< highlight html >}}
$ find . -name index.html | xargs ls -l
-rw-r--r--  1 quoha  staff  0 Sep 29 20:21 ./public/index.html
-rw-r--r--  1 quoha  staff  0 Sep 29 17:31 ./themes/zafta/layouts/index.html
$
{{< /highlight >}}

#### La magia de la estática

Hugo hace dos cosas al generar el sitio. Utiliza plantillas para transformar contenido en HTML y copia archivos estáticos en el sitio. A diferencia del contenido, los archivos estáticos no se transforman. Se copian exactamente como son.

Hugo asume que tu sitio usará CSS y JavaScript, por lo que crea directorios en su tema para mantenerlos. ¿Recuerdas opiniones? Bueno, la opinión de Hugo es que almacenarás tu CSS en un directorio llamado css/ y tu JavaScript en un directorio llamado js/. Si no te gusta, puedes cambiar los nombres de directorio en tu directorio de temas o incluso eliminarlos por completo. Hugo es lo suficientemente amable como para ofrecer su opinión, y luego comportarse bien si no está de acuerdo.

{{< gist naujoel e3d7e8ec4f54003c7cc174bd58ece372 >}}

## El ciclo de desarrollo del tema

Cuando trabajes en un tema, realizarás cambios en el directorio del tema, reconstruirás el sitio y verificarás los cambios en el navegador. Hugo hace esto muy fácil:

1. Purga el directorio public/.
2. Ejecuta el servidor web incorporado en modo watch.
3. Abre tu sitio en un navegador.
4. Actualiza el tema.
5. Echa un vistazo a la ventana de tu navegador para ver los cambios.
6. Regresa al paso 4.

Daré una opinión más: nunca trabajes en un tema en un sitio en vivo. Siempre trabaja en una copia de tu sitio. Realiza cambios en tu tema, pruébalos y luego cópialos en tu sitio. Para mayor seguridad, usa una herramienta como Git para mantener un historial de revisión de tu contenido y tu tema. Créeme cuando digo que es demasiado fácil perder tu mente y tus cambios.

Consulta el sitio oficial de Hugo para obtener información sobre el uso de Git con Hugo.

### Purgar el directorio ```public/```

Al generar el sitio, Hugo creará nuevos archivos y actualizará los existentes en el directorio ```public/```. No eliminará los archivos que ya no se usan. Por ejemplo, los archivos que se crearon en el directorio incorrecto o con el título incorrecto permanecerán. Si los dejas, puedes confundirte con ellos más tarde. Por ello, recomiendo que limpies tu sitio antes de generarlo.

Nota: Si estás construyendo en un SSD, debes ignorar esto. Batir un SSD puede ser costoso.

### La opción Watch de Hugo

La opción ```--watch``` de Hugo supervisará el directorio content/ y los directorios de tus temas en busca de cambios y reconstruirá el sitio automáticamente.

### Recarga en vivo

El servidor web incorporado de Hugo admite la recarga en vivo. A medida que las páginas se guardan en el servidor, se le indica al navegador que actualice la página. Por lo general, esto sucede más rápido de lo que puedes decir: "Wow, eso es totalmente sorprendente".

### Comandos de desarrollo

Usa los siguientes comandos como base para tu flujo de trabajo.

```
## purgar archivos viejos. Hugo recreará el directorio public/.
##
$ rm -rf public
##
## ejecuta Hugo en modo watch
##
$ hugo server --watch --verbose
```
Aquí hay una salida de ejemplo que muestra a Hugo detectando un cambio en la plantilla para la página de inicio. Una vez generado, el navegador web vuelve a cargar la página automáticamente. Ha sucedido antes de decirlo, es increíble.

{{< gist naujoel ed20d66d1e014159330688d1fbb013b4 >}}

## Actualiza la plantilla de la página de inicio

La página de inicio es una de las pocas páginas especiales que Hugo crea automáticamente. Como se mencionó anteriormente, busca uno de los tres archivos en el directorio layout/ del tema:

1. index.html
2. _default/list.html
3. _default/single.html

Podríamos actualizar una de las plantillas predeterminadas, pero una buena decisión de diseño es actualizar la plantilla más específica disponible. Esa no es una regla estricta (de hecho, la romperemos varias veces en este tutorial), pero es una buena generalización.

### Hacer una página de inicio estática

En este momento, esa página está vacía porque no tenemos ningún contenido y no tenemos ninguna lógica en la plantilla. Cambiemos eso agregando algo de texto a la plantilla.

```
$ vi themes/zafta/layouts/index.html
<!DOCTYPE html>
<html>
<body>
  <p>Hugo dice hola!</p>
</body>
</html>
:wq

$
```
Crea el sitio web y luego verifica los resultados.

```
$ hugo --verbose
INFO: 2014/09/29 Using config file: /Users/quoha/Sites/zafta/config.toml
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/themes/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/static/ to /Users/quoha/Sites/zafta/public/
WARN: 2014/09/29 Unable to locate layout: [404.html theme/404.html]
0 draft content
0 future content
0 pages created
0 tags created
0 categories created
in 2 ms

$ find public -type f -name '*.html' | xargs ls -l
-rw-r--r--  1 quoha  staff  78 Sep 29 21:26 public/index.html

$ cat public/index.html
<!DOCTYPE html>
<html>
<body>
  <p>Hugo dice hola!</p>
</html>
```

#### Recarga en vivo

Nota: Si estás ejecutando el servidor con la opción ```--watch```, verás contenido diferente en el archivo:

```
$ cat public/index.html
<!DOCTYPE html>
<html>
<body>
  <p>Hugo dice hola!</p>
<script>document.write('<script src="http://'
        + (location.host || 'localhost').split(':')[0]
    + ':1313/livereload.js?mindelay=10"></'
        + 'script>')</script></body>
</html>
```
Cuando usa ```--watch```, Hugo agrega el script de recarga en vivo. Busca la recarga en vivo en la documentación para ver qué hace y cómo deshabilitarla.

### Crear una página de inicio "dinámica"

"¿Página de inicio dinámica?" Hugo es un generador estático de sitios web, por lo que parece una cosa extraña. Quiero decir, hagamos que la página de inicio refleje automáticamente el contenido del sitio cada vez que Hugo lo construya. Usaremos la iteración en la plantilla para hacer eso.

#### Crear nuevas publicaciones

Ahora que tenemos la página de inicio generando contenido estático, agreguemos algo de contenido al sitio. Mostraremos estas publicaciones como una lista en la página de inicio y también en su propia página.

Hugo tiene un comando para generar una publicación esqueleto, al igual que lo hace para sitios y temas.

```
$ hugo --verbose new post/first.md
INFO: 2014/09/29 Using config file: /Users/quoha/Sites/zafta/config.toml
INFO: 2014/09/29 attempting to create  post/first.md of post
INFO: 2014/09/29 curpath: /Users/quoha/Sites/zafta/themes/zafta/archetypes/default.md
ERROR: 2014/09/29 Unable to Cast <nil> to map[string]interface{}

$
```
Eso no fue muy agradable, ¿verdad?

El comando "new" utiliza un arquetipo para crear el archivo de publicación. Hugo creó un archivo de arquetipo predeterminado vacío, pero eso causa un error cuando hay un tema. Para mí, la solución era crear un archivo de arquetipos específicamente para el tipo de publicación.

```
$ vi themes/zafta/archetypes/post.md
+++
Description = ""
Tags = []
Categories = []
+++
:wq

$ find themes/zafta/archetypes -type f | xargs ls -l
-rw-r--r--  1 quoha  staff   0 Sep 29 21:53 themes/zafta/archetypes/default.md
-rw-r--r--  1 quoha  staff  51 Sep 29 21:54 themes/zafta/archetypes/post.md

$ hugo --verbose new post/first.md
INFO: 2014/09/29 Using config file: /Users/quoha/Sites/zafta/config.toml
INFO: 2014/09/29 attempting to create  post/first.md of post
INFO: 2014/09/29 curpath: /Users/quoha/Sites/zafta/themes/zafta/archetypes/post.md
INFO: 2014/09/29 creating /Users/quoha/Sites/zafta/content/post/first.md
/Users/quoha/Sites/zafta/content/post/first.md created

$ hugo --verbose new post/second.md
INFO: 2014/09/29 Using config file: /Users/quoha/Sites/zafta/config.toml
INFO: 2014/09/29 attempting to create  post/second.md of post
INFO: 2014/09/29 curpath: /Users/quoha/Sites/zafta/themes/zafta/archetypes/post.md
INFO: 2014/09/29 creating /Users/quoha/Sites/zafta/content/post/second.md
/Users/quoha/Sites/zafta/content/post/second.md created

$ ls -l content/post
total 16
-rw-r--r--  1 quoha  staff  104 Sep 29 21:54 first.md
-rw-r--r--  1 quoha  staff  105 Sep 29 21:57 second.md

$ cat content/post/first.md
+++
Categories = []
Description = ""
Tags = []
date = "2014-09-29T21:54:53-05:00"
title = "first"

+++
my first post

$ cat content/post/second.md
+++
Categories = []
Description = ""
Tags = []
date = "2014-09-29T21:57:09-05:00"
title = "second"

+++
my second post

$
```
Crea el sitio web y luego verifica los resultados.

```
$ rm -rf public
$ hugo --verbose
INFO: 2014/09/29 Using config file: /Users/quoha/Sites/zafta/config.toml
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/themes/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 found taxonomies: map[string]string{"category":"categories", "tag":"tags"}
WARN: 2014/09/29 Unable to locate layout: [404.html theme/404.html]
0 draft content
0 future content
2 pages created
0 tags created
0 categories created
in 4 ms
$
```
La salida dice que creó 2 páginas. Esas son nuestras nuevas publicaciones:

```
$ find public -type f -name '*.html' | xargs ls -l
-rw-r--r--  1 quoha  staff  78 Sep 29 22:13 public/index.html
-rw-r--r--  1 quoha  staff   0 Sep 29 22:13 public/post/first/index.html
-rw-r--r--  1 quoha  staff   0 Sep 29 22:13 public/post/index.html
-rw-r--r--  1 quoha  staff   0 Sep 29 22:13 public/post/second/index.html
$
```
Los nuevos archivos están vacíos porque las plantillas utilizadas para generar el contenido están vacías. La página de inicio tampoco muestra el nuevo contenido. Tenemos que actualizar las plantillas para agregar las publicaciones.

### Plantillas individuales y de lista

En Hugo, tenemos tres tipos principales de plantillas. Existe la plantilla de la página de inicio que actualizamos anteriormente. Solo lo usa la página de inicio. También tenemos plantillas "individuales" que se utilizan para generar resultados para un único archivo de contenido. También tenemos plantillas de "lista" que se utilizan para agrupar múltiples piezas de contenido antes de generar resultados.

En términos generales, las plantillas de lista se denominan "list.html" y las plantillas individuales se denominan "single.html".

Hay otros tres tipos de plantillas: parciales, vistas de contenido y términos. No entraremos en muchos detalles sobre estos.

### Agregar contenido a la página de inicio

La página de inicio contendrá una lista de publicaciones. Actualicemos su plantilla para agregar las publicaciones que acabamos de crear. La lógica en la plantilla se ejecutará cada vez que construyamos el sitio.

```
$ vi themes/zafta/layouts/index.html
<!DOCTYPE html>
<html>
<body>
  {{ range first 10 .Data.Pages }}
    <h1>{{ .Title }}</h1>
  {{ end }}
</body>
</html>
:wq

$
```

Hugo usa el motor de plantillas Go. Ese motor escanea los archivos de plantilla en busca de comandos que están encerrados entre "{{" y "}}". En nuestra plantilla, los comandos son:

1. range
2. .Title
3. end

El comando "range" es un iterador. Lo usaremos para pasar por las primeras diez páginas. Cada archivo HTML que crea Hugo se trata como una página, por lo que al recorrer la lista de páginas se verá cada archivo que se creará.

El comando ".Title" imprime el valor de la variable "title". Hugo lo saca de la sección Front Matter del archivo Markdown.

El comando "end" señala el final del iterador de rango. El motor vuelve a la parte superior de la iteración cuando encuentra "end". Todo entre el "range" y el "end" se evalúa cada vez que el motor pasa por la iteración. En este archivo, eso provocaría que el título de las primeras diez páginas salga como encabezado de nivel uno.

Es útil recordar que algunas variables, como .Data, se crean antes de cualquier archivo de salida. Hugo carga cada archivo de contenido en la variable y luego le da a la plantilla la oportunidad de procesar antes de crear los archivos HTML.

Crea el sitio web y luego verifica los resultados.

```
$ rm -rf public
$ hugo --verbose
INFO: 2014/09/29 Using config file: /Users/quoha/Sites/zafta/config.toml
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/themes/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 found taxonomies: map[string]string{"tag":"tags", "category":"categories"}
WARN: 2014/09/29 Unable to locate layout: [404.html theme/404.html]
0 draft content
0 future content
2 pages created
0 tags created
0 categories created
in 4 ms
$ find public -type f -name '*.html' | xargs ls -l
-rw-r--r--  1 quoha  staff  94 Sep 29 22:23 public/index.html
-rw-r--r--  1 quoha  staff   0 Sep 29 22:23 public/post/first/index.html
-rw-r--r--  1 quoha  staff   0 Sep 29 22:23 public/post/index.html
-rw-r--r--  1 quoha  staff   0 Sep 29 22:23 public/post/second/index.html
$ cat public/index.html
<!DOCTYPE html>
<html>
<body>

    <h1>second</h1>

    <h1>first</h1>

</body>
</html>
$
```
Felicidades, la página de inicio muestra el título de las dos publicaciones. Las publicaciones mismas todavía están vacías, pero tomemos un momento para apreciar lo que hemos hecho. Su plantilla ahora genera resultados dinámicamente. Lo creas o no, al insertar el comando range dentro de esas llaves, has aprendido todo lo que necesitas saber para crear un tema. Todo lo que realmente queda es entender qué plantilla se usará para generar cada archivo de contenido y familiarizarse con los comandos para el motor de plantillas.

Y, si eso fuera completamente cierto, este tutorial sería mucho más corto. Hay algunas cosas que debes saber que harán que crear una nueva plantilla sea mucho más fácil. No te preocupes, todo llegará.

### Agregar contenido a las publicaciones

Estamos trabajando con publicaciones, que están en el directorio content/post/. Eso significa que su sección es "post" (y si no hacemos algo extraño, su tipo también es "post").

Hugo usa la sección y el tipo para encontrar el archivo de plantilla para cada pieza de contenido. Hugo buscará primero un archivo de plantilla que coincida con la sección o el nombre del tipo. Si no puede encontrar uno, buscará en el directorio _default/. Hay algunos giros que cubriremos cuando lleguemos a categorías y etiquetas, pero por ahora podemos suponer que Hugo intentará publicar /single.html, luego _default/single.html.

Ahora que conocemos la regla de búsqueda, veamos qué tenemos realmente disponible:

```
$ find themes/zafta -name single.html | xargs ls -l
-rw-r--r--  1 quoha  staff  132 Sep 29 17:31 themes/zafta/layouts/_default/single.html
```
Podríamos crear una nueva plantilla, post/single.html, o cambiar la predeterminada. Como no conocemos ningún otro tipo de contenido, comencemos con la actualización del valor predeterminado.

Recuerda, cualquier contenido para el que no hayamos creado una plantilla terminará usando esta plantilla. Eso puede ser bueno o malo. Malo porque sé que vamos a agregar diferentes tipos de contenido y terminaremos deshaciendo algunos de los cambios que hemos realizado. Es bueno porque podremos ver resultados inmediatos. También es bueno comenzar aquí porque podemos comenzar a construir el diseño básico para el sitio. A medida que agreguemos más tipos de contenido, refactorizaremos este archivo y moveremos la lógica. Hugo lo hace bastante indoloro, así que aceptaremos el costo y procederemos.

Consulta la documentación de Hugo sobre la representación de plantillas para obtener todos los detalles sobre cómo determinar qué plantilla utilizar. Y, como mencionan los documentos, si estás creando un sitio web de aplicación de página única (SPA), puedes eliminar todas las otras plantillas y trabajar solo con la página única predeterminada. Esa es una cantidad refrescante de alegría allí mismo.

#### Actualizar el archivo de plantilla

```
$ vi themes/zafta/layouts/_default/single.html
<!DOCTYPE html>
<html>
<head>
  <title>{{ .Title }}</title>
</head>
<body>
  <h1>{{ .Title }}</h1>
  {{ .Content }}
</body>
</html>
:wq

$
```
Construye el sitio web y verifica los resultados.

```
$ rm -rf public
$ hugo --verbose
INFO: 2014/09/29 Using config file: /Users/quoha/Sites/zafta/config.toml
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/themes/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 found taxonomies: map[string]string{"tag":"tags", "category":"categories"}
WARN: 2014/09/29 Unable to locate layout: [404.html theme/404.html]
0 draft content
0 future content
2 pages created
0 tags created
0 categories created
in 4 ms

$ find public -type f -name '*.html' | xargs ls -l
-rw-r--r--  1 quoha  staff   94 Sep 29 22:40 public/index.html
-rw-r--r--  1 quoha  staff  125 Sep 29 22:40 public/post/first/index.html
-rw-r--r--  1 quoha  staff    0 Sep 29 22:40 public/post/index.html
-rw-r--r--  1 quoha  staff  128 Sep 29 22:40 public/post/second/index.html

$ cat public/post/first/index.html
<!DOCTYPE html>
<html>
<head>
  <title>first</title>
</head>
<body>
  <h1>first</h1>
  <p>my first post</p>

</body>
</html>

$ cat public/post/second/index.html
<!DOCTYPE html>
<html>
<head>
  <title>second</title>
</head>
<body>
  <h1>second</h1>
  <p>my second post</p>

</body>
</html>
$
```
Ten en cuenta que los posts ahora tienen contenido. Puedes ir a localhost:1313/post/first para comprobarlo.

### Enlazando al contenido

Las publicaciones están en la página de inicio. Agreguemos un enlace desde allí a la publicación. Como esta es la página de inicio, actualizaremos su plantilla.

```
$ vi themes/zafta/layouts/index.html
<!DOCTYPE html>
<html>
<body>
  {{ range first 10 .Data.Pages }}
    <h1><a href="{{ .Permalink }}">{{ .Title }}</a></h1>
  {{ end }}
</body>
</html>
```
Construye el sitio web y verifica los resultados.

```
$ rm -rf public
$ hugo --verbose
INFO: 2014/09/29 Using config file: /Users/quoha/Sites/zafta/config.toml
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/themes/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 syncing from /Users/quoha/Sites/zafta/static/ to /Users/quoha/Sites/zafta/public/
INFO: 2014/09/29 found taxonomies: map[string]string{"tag":"tags", "category":"categories"}
WARN: 2014/09/29 Unable to locate layout: [404.html theme/404.html]
0 draft content
0 future content
2 pages created
0 tags created
0 categories created
in 4 ms

$ find public -type f -name '*.html' | xargs ls -l
-rw-r--r--  1 quoha  staff  149 Sep 29 22:44 public/index.html
-rw-r--r--  1 quoha  staff  125 Sep 29 22:44 public/post/first/index.html
-rw-r--r--  1 quoha  staff    0 Sep 29 22:44 public/post/index.html
-rw-r--r--  1 quoha  staff  128 Sep 29 22:44 public/post/second/index.html

$ cat public/index.html
<!DOCTYPE html>
<html>
<body>

    <h1><a href="/post/second/">second</a></h1>

    <h1><a href="/post/first/">first</a></h1>

</body>
</html>

$
```

### Crear un listado de publicaciones

Tenemos las publicaciones que se muestran en la página de inicio y en su propia página. También tenemos un archivo public/post/index.html que está vacío. Hagamos que muestre una lista de todas las publicaciones (no solo las primeras diez).

Necesitamos decidir qué plantilla actualizar. Esta será una lista, por lo que debería ser una plantilla de lista. Echemos un vistazo rápido y veamos qué plantillas de lista están disponibles.

```
$ find themes/zafta -name list.html | xargs ls -l
-rw-r--r--  1 quoha  staff  0 Sep 29 17:31 themes/zafta/layouts/_default/list.html
```

Al igual que con la publicación individual, tenemos que decidir actualizar _default/list.html o crear post/list.html. Todavía no tenemos múltiples tipos de contenido, así que seamos coherentes y actualiza la plantilla de lista predeterminada.

## Crear páginas de nivel superior

Agreguemos una página "Sobre mí" y la mostraremos en el nivel superior (a diferencia de un subnivel como lo hicimos con las publicaciones).

El valor predeterminado en Hugo es utilizar la estructura de directorios del directorio content/ para guiar la ubicación del html generado en el directorio public/. Verifiquemos eso creando una página "Sobre mí" en el nivel superior:

```
$ vi content/about.md
+++
title = "about"
description = "about this site"
date = "2014-09-27"
slug = "about time"
+++

## about us

i'm speechless
:wq
```

Genera el sitio web y verifica los resultados.

```
$ find public -name '*.html' | xargs ls -l
-rw-rw-r--  1 mdhender  staff   334 Sep 27 15:08 public/about-time/index.html
-rw-rw-r--  1 mdhender  staff   527 Sep 27 15:08 public/index.html
-rw-rw-r--  1 mdhender  staff   358 Sep 27 15:08 public/post/first-post/index.html
-rw-rw-r--  1 mdhender  staff     0 Sep 27 15:08 public/post/index.html
-rw-rw-r--  1 mdhender  staff   342 Sep 27 15:08 public/post/second-post/index.html
```

Ten en cuenta que la página no se creó en el nivel superior. Fue creado en un subdirectorio llamado 'about-time/'. Ese nombre vino de nuestro slug. Hugo usará el slug para nombrar el contenido generado. Por cierto, es un valor predeterminado razonable, pero podemos aprender algunas cosas luchando por este archivo.

Otra cosa. Echa un vistazo a la página de inicio.

```
$ cat public/index.html
<!DOCTYPE html>
<html>
<body>
    <h1><a href="http://localhost:1313/post/theme/">creating a new theme</a></h1>
    <h1><a href="http://localhost:1313/about-time/">about</a></h1>
    <h1><a href="http://localhost:1313/post/second-post/">second</a></h1>
    <h1><a href="http://localhost:1313/post/first-post/">first</a></h1>
<script>document.write('<script src="http://'
        + (location.host || 'localhost').split(':')[0]
		+ ':1313/livereload.js?mindelay=10"></'
        + 'script>')</script></body>
</html>
```

¿Te das cuenta de que el enlace "acerca de" aparece en las publicaciones? Eso no es deseable, así que cambiemos eso primero.

```
$ vi themes/zafta/layouts/index.html
<!DOCTYPE html>
<html>
<body>
  <h1>posts</h1>
  {{ range first 10 .Data.Pages }}
    {{ if eq .Type "post"}}
      <h2><a href="{{ .Permalink }}">{{ .Title }}</a></h2>
    {{ end }}
  {{ end }}

  <h1>pages</h1>
  {{ range .Data.Pages }}
    {{ if eq .Type "page" }}
      <h2><a href="{{ .Permalink }}">{{ .Title }}</a></h2>
    {{ end }}
  {{ end }}
</body>
</html>
:wq
```

Genere el sitio web y verifique los resultados. La página de inicio tiene dos secciones, publicaciones y páginas, y cada sección tiene el conjunto correcto de encabezados y enlaces.

Pero esa página acerca de todavía se muestra sobre about-time/index.html.

```
$ find public -name '*.html' | xargs ls -l
-rw-rw-r--  1 mdhender  staff    334 Sep 27 15:33 public/about-time/index.html
-rw-rw-r--  1 mdhender  staff    645 Sep 27 15:33 public/index.html
-rw-rw-r--  1 mdhender  staff    358 Sep 27 15:33 public/post/first-post/index.html
-rw-rw-r--  1 mdhender  staff      0 Sep 27 15:33 public/post/index.html
-rw-rw-r--  1 mdhender  staff    342 Sep 27 15:33 public/post/second-post/index.html
```

Sabiendo que Hugo está usando el slug para generar el nombre del archivo, la solución más simple es cambiar el slug. Hagámoslo de la manera difícil y cambiemos el enlace permanente en el archivo de configuración.

```
$ vi config.toml
[permalinks]
	page = "/:title/"
	about = "/:filename/"
```

Genera el sitio web y verifica que esto no funcionó. Hugo permite que "slug" o "URL" anulen la configuración de enlaces permanentes en el archivo de configuración. Continúa y comenta el slug en content/about.md, luego genera el sitio web para que se cree en el lugar correcto.

## Compartir plantillas

Si has estado siguiendo, probablemente hayas notado que las publicaciones tienen títulos en el navegador y la página de inicio no. Eso es porque no pusimos el título en la plantilla de la página de inicio (layouts/index.html). Es algo fácil de hacer, pero veamos una opción diferente.

Podemos poner los pedazos comunes en una plantilla compartida que se almacena en el directorio themes/zafta/layouts/partials/.

### Crear los parciales de encabezado y pie de página

En Hugo, un parcial es una plantilla recubierta de azúcar. Normalmente, una referencia de plantilla tiene una ruta especificada. Los parciales son diferentes. Hugo los busca a lo largo de una ruta de búsqueda definida TODO. Esto facilita a los usuarios finales anular la presentación del tema.

```
$ vi themes/zafta/layouts/partials/header.html
<!DOCTYPE html>
<html>
<head>
	<title>{{ .Title }}</title>
</head>
<body>
:wq

$ vi themes/zafta/layouts/partials/footer.html
</body>
</html>
:wq
```

### Actualice la plantilla de la página de inicio para usar los parciales

La diferencia más notable entre una llamada de plantilla y una llamada parcial es la falta de ruta:

```
{{ template "theme/partials/header.html" . }}
```
en vez de

```
{{ partial "header.html" . }}
```
Ambos pasan en el contexto.

Cambiemos la plantilla de la página de inicio para usar estos nuevos parciales.

```
$ vi themes/zafta/layouts/index.html
{{ partial "header.html" . }}

  <h1>posts</h1>
  {{ range first 10 .Data.Pages }}
    {{ if eq .Type "post"}}
      <h2><a href="{{ .Permalink }}">{{ .Title }}</a></h2>
    {{ end }}
  {{ end }}

  <h1>pages</h1>
  {{ range .Data.Pages }}
    {{ if or (eq .Type "page") (eq .Type "about") }}
      <h2><a href="{{ .Permalink }}">{{ .Type }} - {{ .Title }} - {{ .RelPermalink }}</a></h2>
    {{ end }}
  {{ end }}

{{ partial "footer.html" . }}
:wq
```

Genera el sitio web y verifica los resultados. El título en la página de inicio ahora es "su título aquí", que proviene de la variable "title" en el archivo config.toml.

### Actualiza la plantilla individual predeterminada para usar los parciales

```
$ vi themes/zafta/layouts/_default/single.html
{{ partial "header.html" . }}

  <h1>{{ .Title }}</h1>
  {{ .Content }}

{{ partial "footer.html" . }}
:wq
```

Genera el sitio web y verifica los resultados. El título de las publicaciones y la página acerca de, ambos deben reflejar el valor en el archivo Markdown.

## Agregar "Fecha de publicación" a las publicaciones

Es común que las publicaciones muestren la fecha en que fueron escritas o publicadas, así que agreguemos eso. El tema principal de nuestras publicaciones tiene una variable llamada "date". Por lo general, es la fecha en que se creó el contenido, pero supongamos que ese es el valor que queremos mostrar.

### Agregar "Fecha de publicación" a la plantilla

Comenzaremos actualizando la plantilla utilizada para representar las publicaciones. El código de la plantilla se verá así:

```
{{ .Date.Format "Mon, Jan 2, 2006" }}
```

Las publicaciones usan la plantilla individual predeterminada, por lo que cambiaremos ese archivo.

```
$ vi themes/zafta/layouts/_default/single.html
{{ partial "header.html" . }}

  <h1>{{ .Title }}</h1>
  <h2>{{ .Date.Format "Mon, Jan 2, 2006" }}</h2>
  {{ .Content }}

{{ partial "footer.html" . }}
:wq
```

Genera el sitio web y verifica los resultados. Las publicaciones ahora tienen la fecha mostrada en ellas. Sin embargo, hay un problema. La página "acerca de" también muestra la fecha.

Como de costumbre, hay un par de maneras de hacer que la fecha se muestre solo en publicaciones. Podríamos hacer una declaración de "si" como lo hicimos en la página de inicio. Otra forma sería crear una plantilla separada para las publicaciones.

La solución "si" funciona para sitios que tienen solo un par de tipos de contenido. También se alinea con el principio del "código para hoy".

Sin embargo, supongamos que hemos hecho que nuestro sitio sea tan complejo que creemos que tenemos que crear un nuevo tipo de plantilla. En Hugo-speak, vamos a crear una plantilla de sección.

Restauremos la plantilla individual predeterminada antes de que la olvidemos.

```
$ mkdir themes/zafta/layouts/post
$ vi themes/zafta/layouts/_default/single.html
{{ partial "header.html" . }}

  <h1>{{ .Title }}</h1>
  {{ .Content }}

{{ partial "footer.html" . }}
:wq
```

Ahora actualizaremos la versión de la publicación de la plantilla individual. Si recuerdas las reglas de Hugo, el motor de plantillas usará esta versión sobre la predeterminada.

```
$ vi themes/zafta/layouts/post/single.html
{{ partial "header.html" . }}

  <h1>{{ .Title }}</h1>
  <h2>{{ .Date.Format "Mon, Jan 2, 2006" }}</h2>
  {{ .Content }}

{{ partial "footer.html" . }}
:wq

```

Ten en cuenta que eliminamos la lógica de fecha de la plantilla predeterminada y la colocamos en la plantilla de publicación. Genera el sitio web y verifica los resultados. Las publicaciones tienen fechas y la página acerca de, no.

### No te repitas

DRY es un buen objetivo de diseño y Hugo hace un gran trabajo al apoyarlo. Parte del arte de una buena plantilla es saber cuándo agregar una nueva plantilla y cuándo actualizar una existente. Mientras te das cuenta de eso, acepta que estarás refactorizando. Hugo lo hace fácil y rápido, por lo que está bien retrasar la división de una plantilla.
