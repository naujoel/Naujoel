---
# Course title, summary, and position.
linktitle: Un curso de ejemplo
summary: Aprende a usar el diseño de documentos para publicar cursos en línea, documentación y tutoriales.
weight: 1

# Page metadata.
title: Overview
date: "2018-09-09T00:00:00Z"
lastmod: "2018-09-09T00:00:00Z"
draft: false  # Is this a draft? true/false
toc: true  # Show table of contents? true/false
type: docs  # Do not modify.

# Add menu entry to sidebar.
# - name: Declare this menu item as a parent with ID `name`.
# - weight: Position of link in menu.
menu:
  example:
    name: Overview
    weight: 1
---

## Flexibilidad

Esta característica se puede usar para publicar contenido como:

* **Cursos online**
* **Documentación**
* **Tutoriales**

La carpeta `courses` se puede renombrar. Por ejemplo, podemos renombrarlo a `docs` para documentación o `tutorials` para crear cursos online.

## Borrar tutoriales

**Para eliminar estas páginas, borra la carpeta `courses` y ver abajo para eliminar el enlace del menú asociado.**

## Actualizar el menú del sitio

Después de renombrar o eliminar la carpeta `courses`, es posible que quieras actualizar cualquier enlace del menú `[[main]]` editando la configuración del menú en `config/_default/menus.toml`.

Por ejemplo, si eliminas esta carpeta, puedes eliminar lo siguiente de la configuración del menú:

```toml
[[main]]
  name = "Courses"
  url = "courses/"
  weight = 50
```

O, si estás creando un sitio de documentación, puedes cambiar el nombre de la carpeta `courses` a` docs` y actualizar la configuración del menú *Courses* asociada a:

```toml
[[main]]
  name = "Docs"
  url = "docs/"
  weight = 50
```

## Actualizar el menú docs

Si utilizas el diseño *docs*, ten en cuenta que el nombre del menú en el front matter debe tener el formato `[menu.X]` donde `X` es el nombre de la carpeta. Por lo tanto, si cambias el nombre de la carpeta `courses/example/`, también debes cambiar el nombre de las definiciones de menú en el front matter de los archivos dentro de `courses/example/` de `[menu.example]` a `[menu.<NombreCarpetaNueva>]`.
