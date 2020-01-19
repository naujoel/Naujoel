---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Comenzando Con Hugo"
subtitle: ""
summary: ""
authors: []
tags: [
  Hugo,
]
categories: [
  Tecnologías,
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
  caption: 'Image credit: [**Hugo**](https://gohugo.io)'
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

## Paso 1. Instala Hugo
Visita [Hugo releases](https://github.com/spf13/hugo/releases) y descarga la versión adecuada para tu sistema operativo y arquitectura.
Guárdalo en un lugar específico ya que lo usaremos en el siguiente paso.
Hay instrucciones más completas disponibles para [instalar Hugo](/overview/installing/)

## Paso 2. Crea los documentos
Hugo tiene su propio sitio de ejemplo que también es el sitio de documentación que está leyendo en este momento.
Siga los siguientes pasos:
 1. Clonar el [repositorio de Hugo](http://github.com/spf13/hugo)
 2. Entra en el repositorio
 3. Ejecuta Hugo en modo servidor y compila los documentos
 4. Abre tu navegador en [http://localhost:1313](http://localhost:1313).

Pseudocomandos correspondientes:

    git clone https://github.com/spf13/hugo
    cd hugo
    /path/to/where/you/installed/hugo server --source=./docs
    > 29 pages created
    > 0 tags index created
    > in 27 ms
    > Web Server is available at http://localhost:1313
    > Press ctrl+c to stop

Una vez que haya llegado aquí, siga el resto de esta página en su compilación local.

## Paso 3. Cambiar el sitio de documentos
Detenga el proceso de Hugo presionando Ctrl+c.
Ahora vamos a ejecutar Hugo nuevamente, pero esta vez con Hugo en modo `watch`.

    /path/to/hugo/from/step/1/hugo server --source=./docs --watch
    > 29 pages created
    > 0 tags index created
    > in 27 ms
    > Web Server is available at http://localhost:1313
    > Watching for changes in /Users/spf13/Code/hugo/docs/content
    > Press ctrl+c to stop

Abra su [editor favorito](http://vim.spf13.com) y cambie una de las páginas de contenido fuente. ¿Qué tal cambiar este mismo archivo para *corregir el error tipográfico*?. ¿Qué tal cambiar este mismo archivo para *corregir el error tipográfico*?.
Los archivos de contenido se encuentran en `docs/content/`. A menos que se especifique lo contrario, los archivos se encuentran en la misma ubicación relativa que la URL, en nuestro caso `docs/content/overview/quickstart.md`.
Cambie y guarde este archivo. Observe lo que sucedió en su terminal.

    > Change detected, rebuilding site
    > 29 pages created
    > 0 tags index created
    > in 26 ms

Actualice el navegador y observe que el error tipográfico ahora está solucionado.
Note lo rápido que fue eso. Intente actualizar el sitio antes de que termine de construirse.. Le reto doblemente. Tener una retroalimentación casi instantánea le permite tener su flujo de creatividad sin esperar construcciones largas.

## Paso 4. Diviértete
El mejor modo de aprender algo es jugar con ello.
