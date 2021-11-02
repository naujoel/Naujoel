---
title: Cómo funciona
linktitle: Cómo funciona Drupal 101 desacoplado
toc: true
type: docs
date: "2020-10-30T00:00:00+01:00"
draft: false
menu:
  decoupled-drupal-101:
    parent: Drupal 101 desacoplado
    weight: 2

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 2
---

Hay mucho entusiasmo en torno a las arquitecturas desacopladas, por lo que antes de embarcarse en un proyecto, es importante hacer un análisis equilibrado. Si elige usar Drupal como repositorio de contenido para servir múltiples aplicaciones, una arquitectura desacoplada podría ser adecuada para usted. Un enfoque desacoplado podría ser la solución adecuada en cualquiera de los dos escenarios siguientes:

1. Un sitio tradicional de Drupal que alimenta uno o más sitios o aplicaciones
2. Un sitio de Drupal sin una interfaz que alimente varios sitios o aplicaciones

Sin embargo, una arquitectura desacoplada puede no ser adecuada para sitios y aplicaciones independientes. Implementar una arquitectura desacoplada en estos casos puede duplicar los flujos de trabajo y obstaculizar los beneficios de una arquitectura Drupal acoplada. Adoptar un enfoque desacoplado por "el bien" de ir desacoplado sin una necesidad clara y justificable puede complicar un proyecto que de otro modo se adaptaría perfectamente a una implementación tradicional de Drupal.

## ¿Cuáles son las diferencias entre arquitecturas desacopladas total y progresivamente?

Mantener una arquitectura CMS acoplada es una opción perfectamente válida para quienes crean sitios y aplicaciones independientes. Sin embargo, si sospecha que sus necesidades van más allá de las ofertas típicas de Drupal, puede seleccionar una estrategia completamente desacoplada o progresivamente desacoplada.

Una arquitectura totalmente desacoplada separa el front-end de Drupal del back end en su totalidad. Hay varias ventajas asociadas con una arquitectura Drupal totalmente desacoplada. Preston So explica tanto las recompensas como los riesgos inherentes a Drupal completamente desacoplado en su blog, The Risks and Rewards of Fully Disoupling Drupal:

- Separación de preocupaciones: Utilizar Drupal estrictamente como un repositorio de contenido puede facilitar una separación de preocupaciones, donde las responsabilidades de la funcionalidad y el modelo de datos se dedican al back-end, mientras que la presentación y la estética se dedican al front-end. Con una arquitectura totalmente desacoplada, el manejo del contenido se limita al back-end. Esto está separado del front-end, que solo aborda la presentación y entrega de ese contenido al usuario final.
- Desarrollo canalizado: esta separación también se extiende a los equipos de back-end y front-end y permite a los desarrolladores trabajar a sus propias velocidades de desarrollo independientes. Los desarrolladores de front-end son libres de controlar el marcado y la renderización, mientras que los desarrolladores de back-end pueden concentrar sus esfuerzos en desarrollar una API RESTful robusta.

## Riesgos de desacoplamiento total

Cuando toda la interfaz está controlada por un marco de JavaScript, los equipos técnicos no pueden aprovechar las capacidades de Drupal que muchos desarrolladores han llegado a conocer y amar. Esta estrategia de desacoplamiento total niega las capacidades de Drupal como la edición en el lugar y la gestión de visualización; también introduce puntos adicionales de falla.

Los riesgos adicionales incluyen:

- Sin protección de scripting entre sitios o desinfección de entrada (especialmente cuando no se usa un marco)
- Sin gestión de diseño y visualización
- Sin flujo de trabajo de contenido previsualizable
- Sin módulos que afecten al front-end
- Sin notificaciones, errores ni mensajes del sistema
- Sin carga progresiva BigPipe ni estrategias avanzadas de almacenamiento en caché
- Sin marcas accesibles o beneficios de experiencia de usuario

## Beneficios de Drupal progresivamente desacoplado

Una solución cada vez más popular para mitigar los riesgos de desacoplar completamente Drupal es una estrategia de desacoplamiento progresivo. A diferencia de una arquitectura totalmente desacoplada, las implementaciones desacopladas progresivamente insertan un marco de JavaScript en la interfaz de un sitio Drupal. Los marcos de JavaScript continúan consumiendo la API REST; sin embargo, ciertas áreas de contenido pueden ser controladas y renderizadas por Drupal, mientras que otras aún pueden aprovechar la renderización del lado del cliente. El desacoplamiento progresivo habilita la experiencia front-end de JavaScript, mientras que los equipos editoriales y técnicos pueden continuar aprovechando las valiosas capacidades de Drupal. Las recompensas de una construcción progresivamente desacoplada mitigan los riesgos inherentes a una arquitectura completamente desacoplada.

## ¿Por qué debería desacoplarse?

En Acquia, nuestro equipo ve una enorme variedad de uso empresarial de Drupal. Hoy en día, las experiencias digitales deben ser omnicanal, interactuar con numerosas aplicaciones y ofrecer una arquitectura basada en API. A continuación se muestran algunos ejemplos de cómo las organizaciones pueden aprovechar Drupal desacoplado para crear experiencias digitales ambiciosas:

**Alimentación de una multitud de dispositivos**: los servicios web pueden enviar datos a cualquier dispositivo digital, no solo a computadoras y teléfonos inteligentes. Junto con la capacidad de Drupal para integrarse con otros sistemas, API-first Drupal, puede servir como un cerebro poderoso para sistemas complejos. Un enfoque de API first coloca a Drupal en el centro de muchos ecosistemas técnicos y simplifica la distribución de contenido entre numerosas aplicaciones.

Sin embargo, muchas de estas aplicaciones tienen sus propios requisitos únicos. Muchos especialistas en marketing han sido condicionados para conceptualizar el contenido en forma de páginas HTML, pero la arquitectura centrada en la página no se aplica a todas las oportunidades de contenido disponibles en la actualidad. Por ejemplo, un Amazon Echo (una interfaz de usuario cero, que es cualquier dispositivo sin una pantalla o pantalla visual) y un sitio web tradicional no entienden el contenido de la misma manera. Los equipos digitales pueden adaptarse a una variedad de canales tratando el contenido más como datos y haciendo la transición hacia modelos de contenido estructurado. El contenido estructurado se refiere a la estrategia de organizar el contenido digital en tipos independientes con campos constituyentes y referencias a otros contenidos. Tratar el contenido como datos estructurados permite a los equipos de marketing crear una vez y publicar en todas partes, a través de numerosos puntos de contacto y canales. La creación de contenido estructurado permite a las organizaciones escalar mejor sus esfuerzos de marketing e interactuar con un cliente en su dispositivo preferido, ya sea la web, una aplicación móvil o Amazon Echo.

Drupal es el mejor CMS para contenido estructurado porque permite una gran personalización de tipos de contenido, campos y metadatos listos para usar. Además, Drupal proporciona excelentes herramientas para administrar entidades de campo, potentes capacidades de taxonomía y etiquetado, y controles de metaetiquetas con todas las funciones.

**Aprovechamiento de otras tecnologías frontales**: los desarrollos recientes en la web han creado una demanda de más flexibilidad en el cliente. Los marcos de JavaScript están ganando popularidad debido a la promesa de una mayor productividad y un código mantenible. Existen muchos, algunos con variaciones en el modelo Modelo-Vista-Controlador (MVC). Algunos de los más populares incluyen Ember, React y Angular. Drupal puede funcionar como una capa de servicios para permitir que el contenido creado en el CMS de Drupal se presente a través de un marco de JavaScript. Este caso de uso es especialmente importante para las agencias digitales, que pueden optar por aprovechar otras tecnologías front-end además de las nativas de Drupal. La sólida colección de servicios web y las API flexibles de Drupal brindan a las agencias digitales libertad técnica y creativa.

**Integración con múltiples sistemas**: Drupal es el CMS elegido por las empresas. Para las empresas con una presencia web permanente, esto a menudo significa convertir propiedades web complejas en sitios web de Drupal. En algunos casos, esto requiere que las organizaciones introduzcan Drupal en el back-end para respaldar los sistemas técnicos existentes.

**Controlar todos los aspectos de los medios**: Drupal, como capa de servicios, puede servir como un repositorio central para enviar videos y datos a los muchos medios disponibles en el mercado de medios actual. Por supuesto, esto incluye aplicaciones nativas de iOS y Android, como se describe en otros ejemplos. Pero también puede incluir el envío de datos a transmisiones televisivas en vivo, la publicación en YouTube y el acceso a futuros medios a medida que estén disponibles.

Para obtener más información sobre cómo Drupal desacoplado puede encajar en su entorno digital, lea API-First Drupal: en camino de publicar una vez, acceder a todas partes.
