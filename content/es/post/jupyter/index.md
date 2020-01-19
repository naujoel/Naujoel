---
title: Mostrar cuadernos Jupyter con Academic
subtitle:
summary: El proyecto Jupyter existe para desarrollar software de código abierto, estándares abiertos y servicios para computación interactiva en docenas de lenguajes de programación.
date: 2019-02-05
lastMod: ""

tags: [
  Academic,
  Hugo,
]
categories: [
  Tecnologías,
]


featured: true
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  placement: 1
  caption: 'Image credit: [**Jupyter**](https://www.freecodecamp.org/news/content/images/2019/08/1_m87_Htb_9Pstq0UcvNJ49w.png)'
  focal_point: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

```python
from IPython.core.display import Image
Image('https://www.python.org/static/community_logos/python-logo-master-v3-TM-flattened.png')
```




![png](./index_1_0.png)




```python
print("Welcome to Academic!")
```

    Welcome to Academic!


## Instala Python y JupyterLab

[Instala Anaconda](https://www.anaconda.com/distribution/#download-section) que incluye Python 3 y JupyterLab.

Alternativamente, instala JupyterLab con `pip3 install jupyterlab`.

## Crea o sube un cuaderno Jupyter

Ejecuta los siguientes comandos en tu terminal, sustituyendo `<MY-WEBSITE-FOLDER>` y `<SHORT-POST-TITLE>` con la ruta del archivo a la carpeta de tu sitio web Academic y un título corto para tu publicación de blog (usa guiones en lugar de espacios), respectivamente:

```bash
mkdir -p <MY-WEBSITE-FOLDER>/content/post/<SHORT-POST-TITLE>/
cd <MY-WEBSITE-FOLDER>/content/post/<SHORT-POST-TITLE>/
jupyter lab index.ipynb
```
El comando `jupyter` anterior lanzará el editor JupyterLab, permitiéndonos agregar metadatos y escribir el contenido.

## Edita los metadatos de tu post

La primera celda de su cuaderno Jupyter contendrá sus metadatos de publicación ([front matter] (https://sourcethemes.com/academic/docs/front-matter/)).

En Jupyter, elija _Markdown_ como el tipo de la primera celda y ajuste sus metadatos en tres guiones, lo que indica que se trata de front matter YAML:

```
---
title: My post's title
date: 2019-09-01

# Put any other metadata here...
---
```
Edite los metadatos de su publicación, utilizando la [documentación](https://sourcethemes.com/academic/docs/managing-content) como guía de las opciones disponibles.

Para configurar una [imagen destacada](https://sourcethemes.com/academic/docs/managing-content/#featured-image), coloque una imagen llamada `Featured` en la carpeta de su publicación.

Para otros consejos, como el uso de las maths, consulte la guía sobre [escribir contenido con Academic](https://sourcethemes.com/academic/docs/writing-markdown-latex/).

## Convertir cuaderno a Markdown

```bash
jupyter nbconvert index.ipynb --to markdown --NbConvertApp.output_files_dir=.
```

## Ejemplo

Esta publicación fue creada con Jupyter. Los archivos originales se pueden encontrar en https://github.com/gcushen/hugo-academic/tree/master/exampleSite/content/post/jupyter
