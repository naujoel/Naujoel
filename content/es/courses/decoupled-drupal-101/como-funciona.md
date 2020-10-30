---
title: Cuándo deberías desacoplar?
linktitle: Cuándo deberías desacoplar Drupal?
toc: true
type: docs
date: "2020-10-30T00:00:00+01:00"
draft: false
menu:
  decoupled-drupal-101:
    parent: Drupal 101 desacoplado
    weight: 1

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 1
---

## ¿Cuál es la diferencia entre una arquitectura tradicional y una desacoplada?

Drupal es un sistema de gestión de contenido que puede respaldar una variedad de aplicaciones desacopladas, como aplicaciones móviles, interfaces de usuario conversacionales como Amazon Echo y pantallas en la tienda. En un CMS tradicional o acoplado, las responsabilidades tanto de front-end como de back-end están contenidas en un solo sistema. El back-end de Drupal está estrechamente acoplado a la presentación, y esto significa que las capas que procesan y entregan datos en plantillas no pueden separarse del back-end de PHP.

Una arquitectura desacoplada permite al desarrollador utilizar otra tecnología para renderizar las experiencias de front-end en lugar de las capas de presentación y tematización que vienen con Drupal listo para usar. Este proceso emplea Drupal como repositorio de contenido, que expone el contenido y los datos para el consumo de otras aplicaciones. Estas aplicaciones podrían incluir:

- Las aplicaciones nativas son aplicaciones desarrolladas para un dispositivo o plataforma específicos, como computadoras de escritorio o dispositivos móviles. Por ejemplo, las aplicaciones móviles a menudo se desarrollan para un dispositivo de teléfono inteligente en particular. Las aplicaciones de iOS y Android se desarrollan en Swift y Java, respectivamente.
- Las aplicaciones JavaScript de una sola página actualizan las páginas dinámicamente a través de solicitudes asincrónicas al servidor y evitan las actualizaciones de páginas completas. Esto significa que las aplicaciones web pueden llamar al servidor sin que el navegador tenga que volver a cargar la página.
- Aplicaciones de Internet de las cosas, que incluyen dispositivos como Amazon Echo, Apple Watch o rastreadores de actividad conectados.

## ¿Cómo funciona una arquitectura desacoplada?

La mayoría de las interacciones que tienen lugar en la web se basan en un paradigma de solicitud / respuesta en el que un usuario solicita datos y un sistema responde reuniendo, formateando y representando el contenido apropiado dentro de una plantilla HTML predefinida. En lugar de que todo esto tenga lugar dentro de un solo sistema, una arquitectura desacoplada distribuye estas responsabilidades entre múltiples sistemas, ya que permite un repositorio de contenido central y una variedad de aplicaciones para intercambiar datos a través de una red.

En una arquitectura desacoplada, el back-end de Drupal actúa como repositorio de contenido. El repositorio de Drupal y la aplicación desacoplada intercambian datos a través de métodos HTTP estándar. Una API de transferencia de estado representacional (REST) ​​es el punto de entrada más común para el repositorio de Drupal, mientras que un cliente HTTP en la aplicación desacoplada es responsable de interpretar las respuestas de la API de REST.

La API REST es una técnica que se utiliza con frecuencia en el desarrollo de servicios web. Una API REST proporciona a los desarrolladores un conjunto de funciones que pueden ejecutar solicitudes y respuestas HTTP entre un servidor y un cliente independientes. En Drupal 8, la API REST está disponible fuera de la caja.

Cuando una aplicación desacoplada emite una solicitud HTTP, la API REST responde con el contenido solicitado. Imagine que la aplicación desacoplada es una nave espacial que se comunica con su control de misión basado en la Tierra (en este caso, el repositorio de Drupal). La llamada y respuesta HTTP son como transmisiones de radio que van y vienen entre la nave espacial y la base. La API REST es el transmisor de la base. El cliente HTTP es la radio de la nave espacial.

Una respuesta HTTP se puede entregar en JSON, XML, además de otras representaciones. En la figura anterior, la API REST y el cliente HTTP actúan como mediadores en la arquitectura desacoplada, lo que permite que tanto los desarrolladores de back-end como los de front-end trabajen con sus marcos preferidos.

## ¿Cuál es la diferencia entre sin cabeza y desacoplado?

En esta guía, hemos optado por utilizar los términos sin cabeza y desacoplado indistintamente. Las distinciones entre sin cabeza y desacopladas son bastante matizadas y pueden ser difíciles de definir. Sin embargo, una buena regla general es la siguiente: todos los CMS sin cabeza están desacoplados, pero no todos los CMS desacoplados son sin cabeza.

En pocas palabras, una arquitectura sin cabeza es la división limpia entre la parte trasera y la delantera. Esto se refiere a la interacción entre un CMS y un front-end.

Una arquitectura desacoplada incluye esta implementación, pero también se extiende a arquitecturas orientadas a servicios. Esto significa que el front-end puede ser selectivo en su comunicación con los diversos componentes del CMS. Por ejemplo, el front-end podría extraer solicitudes del servicio de contenido o del servicio de usuario del back-end de forma independiente. En una arquitectura sin cabeza, el front-end no puede segmentar las solicitudes basándose en estos servicios distintos.

## ¿Qué son los servicios web de Drupal?

Otro término sinónimo de movimiento desacoplado es la capacidad para que las organizaciones sean API first. Tradicionalmente, API first se traduce en construir su API primero y luego desarrollar su aplicación web a su alrededor. Sin embargo, las organizaciones pueden tener varias definiciones de lo que significa para ellas ser API-first. Para Drupal, significa hacer que el contenido almacenado y administrado por Drupal esté disponible para otro software.

Para hacer de Drupal el mejor CMS de código abierto y API, la comunidad de Drupal ha estado trabajando durante muchos años para desarrollar la oferta más sólida de servicios web disponible. Esto es importante porque no todas las aplicaciones desacopladas se comunican a través de una API REST. Para que Drupal sea verdaderamente una API first, los servicios web deben extender la funcionalidad más allá del alcance de la API REST.

Hoy en día, Drupal ofrece una gama de módulos de servicios web, que permiten a cualquiera consumir datos de Drupal con facilidad. Estos incluyen módulos contribuidos además de los módulos que ahora están disponibles en Core (el paquete base estándar que define la última versión de Drupal):

**Servicios web RESTful principales**: con el lanzamiento de D8, Drupal ahora ofrece una API REST lista para usar. Esto incluye operaciones para crear, leer, actualizar y eliminar (CRUD) entidades de contenido y leer entidades de configuración. También hay cuatro módulos REST principales en el núcleo, que incluyen serialización, servicios web RESTful, HAL y autenticación básica. Core REST requiere una configuración limitada al tiempo que proporciona una amplia gama de funciones.

**JSON API**: JSON API está aumentando en popularidad debido a su adopción por parte de los desarrolladores de las comunidades Ruby on Rails y Ember. JSON API es una especificación para las API REST que utilizan el formato JSON y ofrece una funcionalidad más allá de la API REST principal. El módulo JSON API está disponible para Drupal 8.

**GraphQL**: originalmente desarrollado por Facebook, GraphQL es un lenguaje de consulta desarrollado para consultas personalizadas del cliente. GraphQL permite a los clientes de Drupal desacoplado extraer datos fácilmente del back-end, lo que les permite recuperar conjuntos de datos personalizados a través de una sola solicitud. Drupal 8 ahora es compatible con el módulo GraphQL.

## ¿Qué kits de desarrollo de software ofrece Drupal?

Además de una sólida colección de servicios web, Drupal ahora ofrece un ecosistema de kits de desarrollo de software (SDK), que ayudan a acelerar el desarrollo de aplicaciones en otras tecnologías. Los SDK pueden ayudar a ampliar el alcance de Drupal fuera de PHP.

Anteriormente, consumir contenido de Drupal requería cierta comprensión de los detalles de implementación de la API REST. Esto cambia con el módulo Waterwheel de Drupal, que ayuda a los desarrolladores a crear aplicaciones respaldadas por Drupal en JavaScript y Swift, sin necesidad de una amplia experiencia en Drupal:

Waterwheel.js ayuda a los desarrolladores de JavaScript a consultar y manipular datos de Drupal. Waterwheel.js se puede aprovechar universalmente para reutilizar código tanto en el servidor como en el cliente. En el lado del servidor, Waterwheel.js se puede usar para realizar llamadas a la API dentro de Node.js durante la ejecución del lado del servidor de un marco de JavaScript. En el lado del cliente, se puede usar para emitir solicitudes asincrónicas según lo necesite el marco de JavaScript.

Waterwheel.swift brinda soporte a los desarrolladores que crean aplicaciones Swift. Esto incluye la capacidad de consumir la API REST principal de Drupal 8, además de ofrecer capacidades de autenticación y administración de sesiones para aplicaciones Swift. Waterwheel.swift es compatible con iOS, macOS, tvOS y watchOS listo para usar para simplificar la comunicación entre Drupal y las aplicaciones impulsadas por Apple.
