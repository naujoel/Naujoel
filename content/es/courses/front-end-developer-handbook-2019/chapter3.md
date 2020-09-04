---
title: Capítulo 3. Aprendizaje del desarrollador front-end. Recursos (recomendaciones) autodirigidos
linktitle: Capítulo 3. Aprendizaje del desarrollador front-end. Recursos (recomendaciones) autodirigidos
toc: true
type: docs
date: "2020-09-04T00:00:00+01:00"
draft: false
menu:
  front-end-developer-handbook-2019:
    parent: Manual del desarrollador front-end (2019)
    weight: 4

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 4
---

Este capítulo destaca los numerosos recursos (formación en vídeo, libros, etc.) que una persona puede utilizar para dirigir su propio proceso de aprendizaje y su carrera como desarrollador front-end.

Los recursos de aprendizaje identificados (artículos, libros, videos, screencasts, etc.) incluirán material gratuito y de pago. El material pagado se indicará con [$].

## 3.1. - Aprenda Internet / Web

> Internet es un sistema global de redes informáticas interconectadas que utilizan el conjunto de protocolos de Internet (TCP / IP) para conectar varios miles de millones de dispositivos en todo el mundo. Es una red de redes que consta de millones de redes privadas, públicas, académicas, comerciales y gubernamentales de alcance local a global, unidas por una amplia gama de tecnologías de redes electrónicas, inalámbricas y ópticas. Internet lleva una amplia gama de recursos y servicios de información, como los documentos y aplicaciones de hipertexto interconectados de la World Wide Web (WWW), el correo electrónico, la telefonía y las redes de igual a igual para compartir archivos.<br>  
<div class="source">-Wikipedia</div>

![Cómo trabaja internet](/courses/front-end-developer-handbook-2019/chapter3-1.png)

<div class="source">Fuente de la imagen: https://www.helloitsliam.com/2014/12/20/how-the-internet-works-infographic/</div>

- ¿Que es la Internet? [ver]
- Conceptos básicos de Internet [ver]
- Cómo funciona la Web [leer]
- ¿Cómo funciona el internet? https://developer.mozilla.org/en-US/docs/Learn/Common_questions/How_does_the_Internet_work y http://web.stanford.edu/class/msande91si/www-spr04/readings/week1/InternetWhitepaper.htm [leer]
- Cómo funciona Internet [ver]
- Cómo funciona Internet en 5 minutos [ver]
- Cómo funciona la Web [ver]
- ¿Que es la Internet? O, "Tú dices tomate, yo digo TCP / IP" [leer]
- No temas a Internet

![Quién ejecuta internet](/courses/front-end-developer-handbook-2019/chapter3-2.png)

<div class="source">Fuente de la imagen: http://www.bitrebels.com/technology/find-out-who-runs-the-internet-chart/</div>

## 3.2. - Aprender navegadores web

> Un navegador web (comúnmente conocido como navegador) es una aplicación de software para recuperar, presentar y recorrer recursos de información en la World Wide Web. Un recurso de información se identifica mediante un Identificador de recurso uniforme (URI / URL) y puede ser una página web, una imagen, un video u otro contenido. Los hipervínculos presentes en los recursos permiten a los usuarios navegar fácilmente en sus navegadores hacia los recursos relacionados. Aunque los navegadores están diseñados principalmente para usar la World Wide Web, también se pueden usar para acceder a información proporcionada por servidores web en redes privadas o archivos en sistemas de archivos.<br>  
<div class="source">-Wikipedia</div>

Los navegadores más utilizados (en computadoras de escritorio y móviles) son:

1. Chrome (motor: Blink + V8)
2. Firefox (motor: Gecko + SpiderMonkey)
3. Internet Explorer (motor: Trident + Chakra)
4. Safari (motor: Webkit + SquirrelFish)

![Porcentaje de uso de navegadores](/courses/front-end-developer-handbook-2019/chapter3-3.png)

<div class="source">Fuente de la imagen: http://gs.statcounter.com/browser-market-share</div>

### Evolución de los navegadores y las tecnologías web (es decir, API)

- evolutionoftheweb.com [leer]
- Cronología de los navegadores web [leer]

### Los navegadores sin cabeza más utilizados son:

- Chromium sin cabeza (motor: Blink + V8)
- SlimerJS (motor: Gecko + SpiderMonkey)

### Cómo funcionan los navegadores

- 20 cosas que aprendí sobre los navegadores y la Web [leer]
- CSS rápido: cómo diseñan los navegadores las páginas web [leer]
- Cómo funcionan los navegadores: entre bastidores de los navegadores web modernos [leer]
- Quantum Up Close: ¿Qué es un motor de navegador?
- Entonces, ¿cómo procesa realmente el navegador un sitio web? [Ver]
- Qué fuerza el diseño / reflujo [leer]
- Lo que todo desarrollador de frontend debe saber sobre el renderizado de páginas web [leer]

### Optimización para navegadores:

- Optimización de la representación del navegador [ver]
- Optimización del rendimiento del sitio web [ver]

### Comparación de navegadores

- Comparación de navegadores web [leer]

### Hacks del navegador

- browserhacks.com [leer]

### Desarrollo para navegadores

En el pasado, los desarrolladores front-end dedicaban mucho tiempo a hacer que el código funcionara en varios navegadores diferentes. Esto fue una vez un problema más grande de lo que es hoy. Hoy en día, las abstracciones (por ejemplo, React, Webpack, Post-CSS, Babel, etc.) combinadas con los navegadores modernos hacen que el desarrollo del navegador sea bastante fácil. El nuevo desafío no es qué navegador usará el usuario, sino en qué dispositivo ejecutará el navegador.

### Navegadores Evergreen

Las últimas versiones de la mayoría de los navegadores modernos se consideran navegadores perennes. Es decir, en teoría, se supone que se actualizan automáticamente de forma silenciosa sin avisar al usuario. Este movimiento hacia los navegadores que se actualizan automáticamente ha sido una reacción al lento proceso de eliminación de los navegadores más antiguos que no se actualizan automáticamente.

### Elegir un navegador

A día de hoy, la mayoría de los desarrolladores de aplicaciones para el usuario utilizan Chrome y "Chrome Dev Tools" para desarrollar código de aplicaciones. Sin embargo, los navegadores modernos más utilizados ofrecen una variedad de herramientas de desarrollo. Elegir uno para usar en el desarrollo es una elección subjetiva. La cuestión más importante es saber qué navegadores, en qué dispositivos, debe admitir y luego probar adecuadamente.

## 3.3 - Aprenda el sistema de nombres de dominio (también conocido como DNS)

> El sistema de nombres de dominio (DNS) es un sistema de nombres distribuido jerárquicamente para computadoras, servicios o cualquier recurso conectado a Internet o una red privada. Asocia diversa información con los nombres de dominio asignados a cada una de las entidades participantes. Lo más destacado es que traduce nombres de dominio, que los humanos pueden memorizar fácilmente, a las direcciones IP numéricas necesarias para los servicios y dispositivos informáticos en todo el mundo. El sistema de nombres de dominio es un componente esencial de la funcionalidad de la mayoría de los servicios de Internet porque es el servicio de directorio principal de Internet.<br>  
<div class="source">- Wikipedia</div>

![Dónde está x.com](/courses/front-end-developer-handbook-2019/chapter3-4.png)

<div class="source">Fuente de la imagen: http://www.digital-digest.com/blog/DVDGuy/wp-content/uploads/2011/11/how_dns_works.jpg</div>

- Introducción a la terminología, los componentes y los conceptos de DNS [leer]
- DNS explicado [ver]
- Cómo funciona el DNS [leer]
- Internet: direcciones IP y DNS [ver]
- ¿Qué es un nombre de dominio? [leer]

## 3.4 - Aprenda HTTP / Redes (incluidos CORS y WebSockets)

> HTTP: el protocolo de transferencia de hipertexto (HTTP) es un protocolo de aplicación para sistemas de información hipermedia distribuidos y colaborativos. HTTP es la base de la comunicación de datos para la World Wide Web.<br>  
<div class="source">- Wikipedia</div>

### Especificaciones HTTP

- HTTP / 2
- Protocolo de transferencia de hipertexto - HTTP / 1.1

### Documentos HTTP

- MDN HTTP [leer]

### Vídeos / artículos / tutoriales de HTTP

- Redes de navegadores de alto rendimiento: lo que todo desarrollador web debe saber acerca de las redes y el rendimiento web [leer]
- MDN: descripción general de HTTP [leer]
- HTTP: La guía definitiva (Guías definitivas) [leer] [$]
- Preguntas frecuentes sobre HTTP / 2 [leer]
- Conceptos básicos de HTTP [ver] [$]
- Conceptos básicos de HTTP / 2 [ver] [$]
- HTTP: el protocolo que todo desarrollador web debe conocer - Parte 1 [leer]
- HTTP: el protocolo que todo desarrollador web debe conocer - Parte 2 [leer]
- HTTP sucintamente [leer]

### Códigos de estado HTTP

- Códigos de estado HTTP
- Códigos de estado HTTP en 60 segundos [ver]

> CORS: el intercambio de recursos de origen cruzado (CORS) es un mecanismo que permite solicitar recursos restringidos (por ejemplo, fuentes) en una página web desde otro dominio fuera del dominio desde el que se originó el recurso.<br>  
<div class="source">- Wikipedia</div>

### Especificaciones CORS

- Uso compartido de recursos entre orígenes

### CORS

- CORS en acción [leer] [$]
- Control de acceso HTTP (CORS) [leer]

> WebSockets: WebSocket es un protocolo que proporciona canales de comunicación full-duplex a través de una sola conexión TCP. El protocolo WebSocket fue estandarizado por IETF como RFC 6455 en 2011, y la API WebSocket en Web IDL está siendo estandarizada por el W3C.<br>  
<div class="source">- Wikipedia</div>

### WebSockets

- Conecta la Web con WebSockets [ver]
- WebSocket: Comunicaciones ligeras cliente-servidor [leer] [$]
- El protocolo WebSocket [leer]

## 3.5 - Aprenda alojamiento web

> Un servicio de alojamiento web es un tipo de servicio de alojamiento de Internet que permite a las personas y organizaciones hacer que su sitio web sea accesible a través de la World Wide Web. Los servidores web son empresas que proporcionan espacio en un servidor de propiedad o alquilado para su uso por los clientes, además de proporcionar conectividad a Internet, normalmente en un centro de datos.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- Alojamiento web 101: Obtenga su sitio web en vivo en la Web en muy poco tiempo [video]

![Qué es web hosting](/courses/front-end-developer-handbook-2019/chapter3-5.png)

<div class="source">Fuente de la imagen: https://firstsiteguide.com/wp-content/uploads/2016/06/what-is-web-hosting-infographic.jpg</div>

## 3.6 - Aprenda el desarrollo general de front-end

- Frontend Bootcamp / Days in the Web [leer]
- Convertirse en un desarrollador web preparado para una carrera
- Conviértase en desarrollador web front-end [ver] [$]
- Ser desarrollador web [leer]
- freeCodeCamp [interactuar]
  - aprender el desarrollo de front-end durante #100DaysOfCode [leer]
- Nanodegree de desarrollador web front-end [ver] [$]
- Inicio de carrera en desarrollo web front-end [ver] [$]
- Desarrollo web front-end: empezar [ver] [$]
- Inicio rápido del desarrollo web front-end con HTML5, CSS y JavaScript [ver] [$]
- Desarrollo web front-end: la guía de Big Nerd Ranch [leer] [$]
- Introducción completa al desarrollo web [ver] [$]
- Más información sobre desarrollo web front-end [ver] [$]
- Entonces, desea ser un ingeniero de aplicaciones para el usuario [ver]
- codecademy.com: Ruta de desarrollo web [interactuar] [de gratis a $]
- web.dev [leer]

## 3.7 - Aprender diseño de interacción / interfaz de usuario

> **Diseño de interfaz de usuario**: el diseño de interfaz de usuario (UI) o ingeniería de interfaz de usuario es el diseño de interfaces de usuario para máquinas y software, como computadoras, electrodomésticos, dispositivos móviles y otros dispositivos electrónicos, con el objetivo de maximizar la experiencia del usuario. El objetivo del diseño de la interfaz de usuario es hacer que la interacción del usuario sea lo más simple y eficiente posible, en términos de lograr los objetivos del usuario (diseño centrado en el usuario).<br>  
<div class="source">- Wikipedia</div>

> **Patrón de diseño de interacción**: un patrón de diseño es una forma formal de documentar una solución a un problema de diseño común. La idea fue introducida por el arquitecto Christopher Alexander para su uso en planificación urbana y arquitectura de edificios, y se ha adaptado para varias otras disciplinas, incluida la enseñanza y la pedagogía, la organización y el proceso del desarrollo, y la arquitectura y el diseño de software.<br>  
<div class="source">- Wikipedia</div>

> **Diseño de la experiencia del usuario**: el diseño de la experiencia del usuario (UXD o UED o XD) es el proceso de mejorar la satisfacción del usuario mediante la mejora de la usabilidad, la accesibilidad y el placer proporcionado en la interacción entre el usuario y el producto. El diseño de la experiencia del usuario abarca el diseño tradicional de interacción persona-computadora (HCI) y lo extiende al abordar todos los aspectos de un producto o servicio tal como lo perciben los usuarios.<br>  
<div class="source">- Wikipedia</div>

> **Interacción persona-computadora**: La interacción persona-computadora (HCI) investiga el diseño y uso de la tecnología informática, enfocándose particularmente en las interfaces entre personas (usuarios) y computadoras.
Los investigadores en el campo de la HCI observan las formas en que los humanos interactúan con las computadoras y diseñan tecnologías que permiten a los humanos interactuar con las computadoras de formas novedosas.<br>  
<div class="source">- Wikipedia</div>

Como mínimo, sugeriría leer los siguientes textos canónicos sobre el tema para poder apoyar y construir interfaces de usuario utilizables.

- Acerca de la cara: lo esencial del diseño de interacción [leer] [$]
- Diseño para piratas informáticos: belleza de ingeniería inversa [leer] [$]
- Diseño para no diseñadores [ver]
- Diseño de interfaces [leer] [$]
- Diseño de interfaces web: principios y patrones para interacciones enriquecidas [leer] [$]
- Don't Make Me Think, Revisited: Un enfoque de sentido común para la usabilidad web [leer] [$]

## 3.8 - Aprenda HTML y CSS

> **HTML**: el lenguaje de marcado de hipertexto, comúnmente conocido como HTML, es el lenguaje de marcado estándar que se utiliza para crear páginas web. Los navegadores web pueden leer archivos HTML y convertirlos en páginas web visibles o audibles. HTML describe la estructura de un sitio web semánticamente junto con pistas para la presentación, lo que lo convierte en un lenguaje de marcado, en lugar de un lenguaje de programación.<br>  
<div class="source">- Wikipedia</div>

> **CSS**: hojas de estilo en cascada (CSS) es un lenguaje de hojas de estilo que se utiliza para describir el aspecto y el formato de un documento escrito en un lenguaje de marcado. Aunque se utiliza con mayor frecuencia para cambiar el estilo de las páginas web y las interfaces de usuario escritas en HTML y XHTML, el lenguaje se puede aplicar a cualquier tipo de documento XML, incluidos XML simple, SVG y XUL. Junto con HTML y JavaScript, CSS es una tecnología fundamental utilizada por la mayoría de los sitios web para crear páginas web visualmente atractivas, interfaces de usuario para aplicaciones web e interfaces de usuario para muchas aplicaciones móviles.<br>  
<div class="source">- Wikipedia</div>

Al igual que con la construcción de una casa, se podría considerar HTML como marco y CSS como pintura y decoración.

### Aprendizaje general:

- Centrado absoluto en CSS [leer]
- Posicionamiento CSS [ver] [$]
- Introducción al desarrollo web (v2) [ver] [$] - Desarrollo web front-end: comenzar [ver] [$]
- Inicio rápido del desarrollo web front-end con HTML5, CSS y JavaScript [ver] [$]
- HTML y CSS: diseño y creación de sitios web [leer] [$]
- Flujo de documentos HTML [ver] [$]
- Dominio de HTML: semántica, estándares y estilo [leer] [$]
- Interneting es difícil [leer]
- Introducción a HTML / CSS: creación de páginas web [ver]
- Aprenda a codificar HTML y CSS [leer]
- Aprenda el diseño CSS [leer]
- MarkSheet [leer]
- MDN: HTML [leer]
- MDN: CSS [leer]
- HTML semántico: cómo estructurar páginas web [ver]
- Estructura sólida de formulario HTML [ver]
- Comprensión del modelo de caja CSS [ver]
- Diseño web resiliente [leer]

### Dominar CSS:

- Una guía completa de Flexbox [leer]
- CSS Grids y Flexbox para diseño web adaptable [ver] [$]
- CSS Diner [interactuar]
- Selectores de CSS desde CSS4 hasta CSS1 [leer]
- Secretos de CSS: mejores soluciones para los problemas cotidianos de diseño web [leer] [$]
- CSS3 [leer]
- CSS en profundidad, v2 [ver] [$]
- ¿Qué es el Flexbox? Un curso de 20 videos simple y gratuito que lo ayudará a dominar CSS y
Flexbox [ver]
- 30 Seconds of CSS: una colección cuidada de fragmentos de CSS útiles que puede comprender en 30 segundos o menos. [leer]

### Referencias / Documentos:

- CSS Triggers ... un juego de diseño, pintura y composición
- cssreference.io
- cssvalues.com
- CSS predeterminado para el navegador Chrome
- Head: una lista de todo lo que podría incluirse en el head de tu documento
- Referencia de atributos HTML
- Referencia CSS de MDN
- Referencia de elementos HTML de MDN

### Glosario / Vocabulario:

- Glosario de CSS: referencia de programación para comentarios, propiedades y selectores de cobertura de CSS
- Vocabulario CSS
- Referencia de programación del glosario HTML para elementos HTML

### Estándares / Especificaciones:

- Todas las especificaciones CSS del W3C
- Todas las especificaciones HTML del W3C
- Especificación de hojas de estilo en cascada Nivel 2 Revisión 2 (CSS 2.2)
- Índices CSS: una lista de todos los términos definidos por las especificaciones CSS
- Los elementos de HTML de los atributos globales del estándar de vida
- La sintaxis HTML de Living Standard HTML 5.2 de W3C
- Selectores Nivel 3

### Arquitectura de CSS:

- Diseño atómico [leer]
- BEM
- ITCSS
- OOCSS [leer]
- SMACSS [leer] [$]
  - Arquitectura modular escalable para CSS (SMACSS) [ver] [$]
- SUIT CSS
- rscss

### Convenciones de autoría / arquitectura:

- Guía de código CSS [leer]
- css-arquitectura
- cssguidelin.es [leer]
- CSS idiomático [leer]
- MaintainableCSS [leer]
- Estándares para desarrollar HTML y CSS flexibles, duraderos y sostenibles [leer]

## 3.9 - Aprenda la optimización de motores de búsqueda

> La optimización de motores de búsqueda (SEO) es el proceso de afectar la visibilidad de un sitio web o una página web en los resultados no pagados de un motor de búsqueda, a menudo denominados resultados "naturales", "orgánicos" o "obtenidos". En general, cuanto más temprano (o mejor clasificado en la página de resultados de búsqueda), y con más frecuencia aparezca un sitio en la lista de resultados de búsqueda, más visitantes recibirá de los usuarios del motor de búsqueda. El SEO puede apuntar a diferentes tipos de búsqueda, incluida la búsqueda de imágenes, la búsqueda local, la búsqueda de videos, la búsqueda académica, la búsqueda de noticias y los motores de búsqueda verticales específicos de la industria.<br>  
<div class="source">- Wikipedia</div>

![SEO explicado](/courses/front-end-developer-handbook-2019/chapter3-6.png)

<div class="source">Fuente de la imagen: https://visual.ly/community/infographic/computers/how-does-seo-work</div>

### Aprendizaje general:

- Guía de inicio de optimización de motores de búsqueda de Google [leer]
- SEO moderno [reloj] [$]
- Conceptos básicos de SEO de David Booth [ver] [$]
- Conceptos básicos de SEO de Paul Wilson [ver] [$]
- Tutorial de SEO para principiantes en 2016 [leer]
- SEO para diseñadores web [ver] [$]

## 3.10 - Aprenda JavaScript

> JavaScript es un lenguaje de programación de alto nivel, dinámico, sin tipo e interpretado. Se ha estandarizado en la especificación del lenguaje ECMAScript. Junto con HTML y CSS, es una de las tres tecnologías esenciales de la producción de contenido en la World Wide Web; la mayoría de los sitios web lo utilizan y es compatible con todos los navegadores web modernos sin complementos. JavaScript está basado en prototipos con funciones de primera clase, lo que lo convierte en un lenguaje de múltiples paradigmas, que admite estilos de programación orientados a objetos, imperativos y funcionales. Tiene una API para trabajar con texto, matrices, fechas y expresiones regulares, pero no incluye ninguna E / S, como redes, almacenamiento o instalaciones de gráficos, confiando para estos en el entorno host en el que está integrado.<br>  
<div class="source">- Wikipedia</div>

### Empezando:

- MDN: JavaScript [leer]
- javascript.info
- Ilustración de JavaScript [leer]
- JavaScript elocuente [leer]

### Aprendizaje general:

- Hablando JavaScript [leer]
- JavaScript para programadores impacientes [leer]
- No conoces JS: Up & Going [leer]
- No conoces JS: tipos y gramática [leer]
- No conoces JS: alcance y cierres [leer]
- No conoces JS: esto y prototipos de objetos [leer]
- Hoja de referencia de JavaScript moderna: hoja de referencia para JavaScript, conocimiento que encontrará con frecuencia en proyectos modernos. [leer]
- JavaScript: Las partes difíciles [ver] [$]
- Fundamentos profundos de JavaScript (v3) [ver] [$]

### Masterización:

- Configuración de ES6 [leer]
- ES6 PARA TODOS! [ver] [$]
- Explorando ES6 [leer]
- No conoces JS: ES6 y más allá [leer]
- Comprensión de ECMAScript 6: la guía definitiva para desarrolladores de JavaScript [leer] [$]
- JavaScript: The Recent Parts [ver] [$]
- Explorando ES2016 y ES2017 [leer]
- Explorando ES2018 y ES2019 [leer]
- Ilustración de expresiones regulares de JavaScript [leer]
- Uso de expresiones regulares [watch] [$]
- No conoces JS: Async y rendimiento [leer]
- JavaScript con promesas [leer] [$]
- Desarrollo de JavaScript basado en pruebas [leer] [$]
- JS MythBusters [leer]
- Robusto JavaScript [leer]
- Algoritmos JavaScript y estructuras de datos [leer]
- 33 conceptos que todo desarrollador de JavaScript debe conocer [leer]
- doesitmutate.xyz [leer]

### JavaScript funcional:

- Jerga de programación funcional
- funfunfunction: Programación funcional en JavaScript [ver]
- Functional-Light-JS [leer]
- Programación funcional en JavaScript: cómo mejorar sus programas JavaScript mediante técnicas funcionales [leer]
- Guía principalmente adecuada para FP (en javascript) [leer]
- El profesor Frisby presenta JavaScript funcional componible [ver]
- JavaScript Allongé [leer] [$]
- JavaScript funcional-ligero (v2) [ver] [$]
- Programación funcional incondicional en JavaScript [ver] [$]

### Referencias / Documentos:

- Referencia de JavaScript de MDN
- Referencia de JavaScript de MSDN

### Glosario / Enciclopedia / Jerga:

- La enciclopedia de JavaScript
- Glosario de JavaScript
- Jerga JavaScript simplificada

### Estándares / especificaciones:

- Cómo leer la especificación ECMAScript
- Especificación de idioma ECMAScript® 2015
- Especificación de idioma ECMAScript® 2016
- Especificación de idioma ECMAScript® 2017
- Especificación de idioma ECMAScript® 2018
- Especificación de idioma ECMAScript® 2019
- Estado, proceso y documentos para ECMA262

### Estilo:

- Guía de estilo de JavaScript de Airbnb
- Estilo estándar de JavaScript
- Estilo semi-estándar de JavaScript

### Recursos de aprendizaje JS obsoletos:

- Crockford en JavaScript - Volumen 1: Los primeros años [ver]
- Crockford en JavaScript - Capítulo 2: Y luego estaba JavaScript [ver]
- Crockford en JavaScript - Acto III: Función máxima [ver]
- Crockford en JavaScript - Episodio IV: La metamorfosis de Ajax [ver]
- Crockford en JavaScript - Parte 5: El fin de todas las cosas [ver]
- Crockford en JavaScript - Escena 6: Loopage [ver]
- Patrones de JavaScript [leer] [$]
- Los principios de JavaScript orientado a objetos [leer] [$]
- Módulos de JavaScript [leer]
- JavaScript funcional: introducción a la programación funcional con Underscore.js [leer] [$]
- Las partes buenas de JavaScript y la Web [ver] [$]
- JavaScript de alto rendimiento (crear interfaces de aplicaciones web más rápidas) [leer] [$]

### Exploradores / visualizadores de JS:

- Explorador de matrices de JavaScript
- Explorador de objetos JavaScript
- Visualizador de JavaScript

## 3.11 - Aprenda DOM, BOM, CSSOM y jQuery

> **DOM**: el modelo de objetos de documento (DOM) es una convención multiplataforma e independiente del lenguaje para representar e interactuar con objetos en documentos HTML, XHTML y XML. Los nodos de cada documento están organizados en una estructura de árbol, llamada árbol DOM. Los objetos en el árbol DOM se pueden direccionar y manipular utilizando métodos en los objetos. La interfaz pública de un DOM se especifica en su interfaz de programación de aplicaciones (API).<br>  
<div class="source">- Wikipedia</div>

> **BOM**: el modelo de objetos del navegador (BOM) es una convención específica del navegador que se refiere a todos los objetos expuestos por el navegador web. A diferencia del Modelo de objetos de documento, no existe un estándar de implementación ni una definición estricta, por lo que los proveedores de navegadores son libres de implementar la lista de materiales de la forma que deseen.<br>  
<div class="source">- Wikipedia</div>

> **jQuery**: jQuery es una biblioteca de JavaScript multiplataforma diseñada para simplificar la creación de scripts de HTML en el lado del cliente. jQuery es la biblioteca de JavaScript más popular en uso en la actualidad, con instalación en el 65% de los 10 millones de sitios con mayor tráfico en la Web. jQuery es un software gratuito de código abierto con licencia MIT.<br>  
<div class="source">- Wikipedia</div>

La ruta ideal, pero ciertamente la más difícil, sería aprender primero JavaScript, luego DOM, luego jQuery. Sin embargo, haz lo que tenga sentido para tu cerebro. La mayoría de los desarrolladores de aplicaciones para el usuario aprenden sobre JavaScript y luego sobre DOM aprendiendo primero jQuery. Cualquiera sea el camino que tome, asegúrese de que JavaScript, DOM y jQuery no se conviertan en una caja negra.

### Aprendizaje general:

- El modelo de objetos de documento [leer]
- HTML / JS: hacer que las páginas web sean interactivas [ver]
- HTML / JS: hacer que las páginas web sean interactivas con jQuery [ver]
- jQuery Enlightenment [leer]
- ¿Qué es el DOM? [leer]

### Masterización:

- Scripting DOM avanzado: Técnicas de diseño web dinámico [leer] [$]
- Conceptos básicos de JS avanzados para jQuery y scripts de DOM puro [ver] [$]
- Douglas Crockford: una API incómoda: la teoría del DOM [ver]
- DOM Enlightenment [leer] [$] o leer en línea gratis
- Corrección de errores comunes de jQuery [ver] [$]
- JavaScript sin jQuery [ver] [$]
- Consejos y trucos de jQuery [ver] [$]

### Referencias / Documentos:

- jQuery Docs
- Eventos
- Compatibilidad con el navegador DOM
- Compatibilidad con el navegador de eventos DOM
- Compatibilidad con el navegador de interfaces HTML
- Modelo de objetos de documento (DOM) de MDN
- Modelo de objetos del navegador MDN
- Modelo de objetos de documento MDN
- Referencia de eventos de MDN
- Modelo de objetos de documento (DOM) de MSDN
- Modelo de objetos CSS (CSSOM)

### Estándares / Especificaciones:

- Modelo de objetos de documento (DOM) Nivel 3 Especificación de eventos
- Informes técnicos del modelo de objetos de documento (DOM)
- Estándar de vida DOM
- W3C DOM4

## 3.12 - Aprenda animación web

### Aprendizaje general:

- SVG Essentials and Animation, v2 [$] [ver]
- Aventuras en animaciones web [$] [ver]
- Animando con Snap.svg [$] [ver]
- Animación en CSS3 y HTML5 [$] [ver]
- Crear animaciones en CSS [leer y mirar]
- Animación CSS en el mundo real [$] [ver]
- Animación básica HTML5 con JavaScript [$] [leer]
- Aprenda a crear animaciones en JavaScript [leer y mirar]
- Motion Design con CSS [$] [ver]
- Estado de la animación 2015 [ver]
- Animación web con JavaScript: desarrollo y diseño (desarrollo y diseño) [$] [leer]

### Estándares / Especificaciones:

- Animaciones web

## 3.13 - Aprenda fuentes, iconos e imágenes web

> La tipografía web se refiere al uso de fuentes en la World Wide Web. Cuando se creó HTML por primera vez, las fuentes y estilos de fuente se controlaban exclusivamente mediante la configuración de cada navegador web. No había ningún mecanismo para que las páginas web individuales controlaran la visualización de fuentes hasta que Netscape introdujo la etiqueta <font> en 1995, que luego se estandarizó en la especificación HTML 3.2. Sin embargo, la fuente especificada por la etiqueta tenía que estar instalada en la computadora del usuario o se usaría una fuente alternativa, como la fuente sans-serif o monoespacio predeterminada de un navegador. La primera especificación de Hojas de estilo en cascada se publicó en 1996 y proporcionó las mismas capacidades.<br>
La especificación CSS2 se lanzó en 1998 e intentó mejorar el proceso de selección de fuentes agregando coincidencia de fuentes, síntesis y descarga. Estas técnicas no se utilizaron mucho y se eliminaron en la especificación CSS2.1. Sin embargo, Internet Explorer agregó soporte para la función de descarga de fuentes en la versión 4.0, lanzada en 1997. La descarga de fuentes se incluyó más tarde en el módulo de fuentes CSS3 y desde entonces se implementó en Safari 3.1, Opera 10 y Mozilla Firefox 3.5. Posteriormente, esto ha aumentado el interés en la tipografía web, así como en el uso de la descarga de fuentes.<br>  
<div class="source">- Wikipedia</div>

### Fuentes:

- Una guía completa sobre las estrategias de carga de fuentes [leer]
- Beautiful Web Type una muestra de los mejores tipos de letra del directorio de fuentes web de Google [leer]
- Guía rápida de fuentes web a través de @font-face [leer]
- MDN: fuentes web [leer]
- Tipografía web adaptable, v2 [ver] [$]
- Tipografía para la Web [ver] [$]

### Iconos:

- [leer] [ver]

### Imágenes:

- MDN: imágenes en HTML [leer]
- MDN: imágenes adaptables [leer]
- SVG EN LA WEB - Una guía práctica [leer]

## 3.14 - Aprenda accesibilidad

> La accesibilidad se refiere al diseño de productos, dispositivos, servicios o entornos para personas con discapacidad. El concepto de diseño accesible asegura tanto el "acceso directo" (es decir, sin asistencia) como el "acceso indirecto", lo que significa compatibilidad con la tecnología de asistencia de una persona (por ejemplo, lectores de pantalla de computadora).<br>
La accesibilidad puede verse como la "capacidad de acceder" y beneficiarse de algún sistema o entidad. El concepto se centra en permitir el acceso de personas con discapacidades o necesidades especiales, o permitir el acceso mediante el uso de tecnología de asistencia; sin embargo, la investigación y el desarrollo en accesibilidad trae beneficios para todos.<br>
La accesibilidad no debe confundirse con la usabilidad, que es la medida en que un producto (como un dispositivo, servicio o entorno) puede ser utilizado por usuarios específicos para lograr objetivos específicos con eficacia, eficiencia y satisfacción en un contexto de uso específico. La accesibilidad está fuertemente relacionada con el diseño universal, que es el proceso de creación de productos que sean utilizables por personas con la gama más amplia de habilidades posibles, que operen dentro de la gama más amplia de situaciones posibles. Se trata de hacer que las cosas sean accesibles para todas las personas (tengan o no una discapacidad).<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- 9 consejos para obtener el mínimo de accesibilidad web
- Fundamentos de UX: accesibilidad [ver] [$]
- Cómo los lectores de pantalla admiten los elementos HTML [leer]
- Introducción a la accesibilidad web - WAI [leer]
- Diseño universal para aplicaciones web: aplicaciones web que llegan a todos [leer] [$]
- Accesibilidad web: introducción [ver] [$]
- Una Web para todos [leer] [$]
- Accesibilidad web [ver] [$]
- A11ycasts [ver]
- Accesibilidad de Google: curso de Udacity [ver]

### Estándares / Especificaciones:

- Estado actual de las aplicaciones de Internet enriquecidas accesibles (WAI-ARIA)
- Iniciativa de accesibilidad web (WAI)
- Estado actual de las Pautas de accesibilidad al contenido web (WCAG)

## 3.15 - Aprenda las API web / del navegador

![APIs de navegador](/courses/front-end-developer-handbook-2019/chapter3-7.png)

<div class="source">Fuente de la imagen: http://www.evolutionoftheweb.com/</div>

El BOM (modelo de objetos de navegador) y el DOM (modelo de objetos de documento) no son las únicas API de navegador que están disponibles en la plataforma web dentro de los navegadores. Todo lo que no es específicamente el
DOM o BOM, como una interfaz para programar el navegador podría considerarse una API web o del navegador (trágicamente en el pasado, algunas de estas API se han llamado API HTML5, lo que confunde sus propias especificaciones/estandarización con la especificación HTML5 real que especifica el lenguaje de marcado HTML5).

Tenga en cuenta que las API web o del navegador incluyen API de dispositivo (por ejemplo, Navigator.getBattery()) que están disponibles a través del navegador en dispositivos de tableta y teléfono.

Debe conocer y aprender, cuando corresponda, las API de web/navegador. Una buena herramienta para familiarizarse con todas estas API sería investigar los resultados de HTML5test.com para los 5 navegadores más actuales.

MDN tiene una gran cantidad de información sobre API web / navegador.

- Referencia de la API web de MDN
- Referencia de la interfaz de las API web de MDN: todas las interfaces, ordenadas alfabéticamente
- MDN WebAPI: enumera las API de acceso a dispositivos y otras API útiles para aplicaciones

Tenga en cuenta que no todas las API están especificadas por el W3C o WHATWG.

Además de MDN, es posible que los siguientes recursos le resulten útiles para conocer todas las API de web/navegador:

- El índice de la API de JavaScript HTML 5
- Descripción general de HTML5
- platform.html5.org

## 3.16 - Aprenda JSON (notación de objetos JavaScript)

> JSON, (pronunciado canónicamente a veces Notación de objetos JavaScript), es un formato estándar abierto que utiliza texto legible por humanos para transmitir objetos de datos que constan de pares atributo-valor. Es el formato de datos principal utilizado para la comunicación asincrónica entre navegador y servidor (AJAJ), y reemplaza en gran medida a XML (utilizado por AJAX).<br>
Aunque originalmente se deriva del lenguaje de secuencias de comandos de JavaScript, JSON es un formato de datos independiente del lenguaje. El código para analizar y generar datos JSON está disponible en muchos lenguajes de programación.<br>
El formato JSON fue especificado originalmente por Douglas Crockford. Actualmente está descrito por dos estándares competidores, RFC 7159 y ECMA-404. El estándar ECMA es mínimo, y describe solo la sintaxis gramatical permitida, mientras que el RFC también proporciona algunas consideraciones semánticas y de seguridad. El tipo de medio oficial de Internet para JSON es application/json. La extensión del nombre de archivo JSON es .json.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- Introducción a la notación de objetos de JavaScript: una guía precisa para JSON [leer] [$]
- json.com [leer]
- ¿Qué es JSON? [ver]

### Referencias / Documentos:

- json.org [leer]

### Estándares / Especificaciones:

- ECMA-404 El formato de intercambio de datos JSON
- RFC 7159 El formato de intercambio de datos de la notación de objetos JavaScript (JSON)
- STD 90 - RFC 8259 - El intercambio de datos de la notación de objetos JavaScript (JSON)
Formato, DICIEMBRE 2017

### Arquitectura:

- API JSON

## 3.17 - Aprenda las plantillas JS

Por lo general, se usa una plantilla de JavaScript, pero no siempre con una solución MV* para separar partes de la vista (es decir, la interfaz de usuario) de la lógica y el modelo (es decir, los datos o JSON).

- ES6 Template Literals, ¿el asesino de los manillares? [leer]
- Empezando con nunjucks [leer]
[leer] [$]
- Plantillas Lodash [docs]

Tenga en cuenta que JavaScript 2015 (también conocido como ES6) agregó un mecanismo de plantillas nativo llamado "Plantillas de cadenas". Además, las plantillas en los últimos tiempos han sido reemplazadas por cosas como JSX, un elemento de plantilla o cadenas HTML.

Si no estuviera usando React & JSX, primero buscaría plantillas de JavaScript
strings "y cuando eso faltaba pasar a nunjucks.

## 3.18 - Aprenda generadores de sitios estáticos

Los generadores de sitios estáticos, generalmente escritos usando código del lado del servidor (es decir, ruby, php, python, nodeJS, etc.), producen archivos HTML estáticos a partir de texto/datos estáticos + plantillas que están destinadas a enviarse desde un servidor al cliente de forma estática sin una naturaleza dinámica.

### Aprendizaje general:

- JAMstack [leer]
- Generadores de sitios estáticos [leer]
- Trabajar con sitios estáticos: llevar el poder de la simplicidad a los sitios modernos [leer] [$]

## 3.19 - Aprenda informática a través de JS

- Cuatro semestres de informática en seis horas [video] [$]
- Cuatro semestres de informática en seis horas: Parte 2 [video] [$]
- Ciencias de la computación en JavaScript [leer]
- Colección de paradigmas, algoritmos y enfoques clásicos de la informática escritos en JavaScript [leer]
- Una guía práctica de algoritmos con JavaScript [ver] [$]
- Introducción a las estructuras de datos para entrevistas [ver] [$]
- Clase magistral de estructuras de datos y algoritmos JavaScript [ver] [$]

## 3.20 - Aprenda la arquitectura de aplicaciones front-end

### Aprendizaje general:

- Agarre la guía de interfaz [leer]
- Un conjunto de mejores prácticas para proyectos de JavaScript
- Libro de hechizos del desarrollador web moderno
- Pila de JavaScript desde cero

### Materiales de aprendizaje obsoletos:

- Diseño de aplicaciones JavaScript [leer] [$]
- Cree una aplicación con React y Ampersand [ver]
- Guía de campo para aplicaciones web [leer]
- Cuestionario de directrices de frontend [leer]
- JavaScript humano [leer]
- Nicholas Zakas: Arquitectura de aplicaciones JavaScript escalable [ver]
- Organizar la funcionalidad de JavaScript [ver] [$]
- Patrones para la arquitectura de aplicaciones JavaScript a gran escala [leer]
- Genial [leer]
- Estudios de caso de frontend [leer]

Últimamente no se está creando mucho contenido general sobre este tema. La mayor parte del contenido que se ofrece para aprender a crear aplicaciones front-end/SPA/JavaScript presupone que ha elegido una herramienta como Angular, Ember, React o Aurelia.

Mi consejo, en 2019 aprenda React y Mobx y Apollo/graphql.

## 3.21 - Aprenda Data (es decir, JSON) API Design

- Diseño de API, v3 [ver] [$]
- Cree API que no odiará [$] [leer]
- API JSON [leer]

## 3.22 - Aprender Reaccionar

### Aprenda React:

- Tutorial: Introducción a reaccionar [leer]
- ReactJS para gente estúpida [leer]
- La guía para principiantes de ReactJS [ver]
- Introducción completa a React v4 [ver] [$]
- React [leer]
- Suscripción de video de React Patterns [ver] [$]
- React Enlightenment [leer]
- TUTORIAL DE REACT JS # 1 - Introducción a Reactjs Javascript y configuración del espacio de trabajo [ver]

### Dominando React:

- Cree su primera aplicación React de calidad de producción [ver] [$]
- Patrones avanzados de componentes de React [ver] [$]
- React intermedio [ver] [$]
- Patrones React [leer]
- 8 decisiones clave del componente React [leer]
- React - Conceptos teóricos básicos [leer]
- Base de código de React + Mobx que contiene ejemplos del mundo real (CRUD, autenticación, patrones avanzados, etc.) que se adhieren a las especificaciones y API de RealWorld. [código]
- Introducción a React Router v4 y su filosofía hacia el enrutamiento [leer]

Una vez que tenga un buen manejo de React, continúe con el aprendizaje de una solución de administración de estado más sólida como MobX. Si eres un desarrollador experimentado con conocimientos de programación funcional, mira Redux. Si necesita ayuda para comprender el papel de la administración de estado más allá de ver setState de React, "Administración de estado avanzada en React (con Redux y MobX)".

## 3.23 - Aprenda la gestión del estado de la aplicación

- Gestión de estado en JavaScript [leer]
- Gestión avanzada del estado en React (con Redux y MobX) [ver] [$]
- Tutorial de React js - Cómo funciona Redux [ver]
- MobX + React es IMPRESIONANTE [ver]

## 3.24 - Aprenda la aplicación web progresiva

> A diferencia de las aplicaciones tradicionales, las aplicaciones web progresivas son un híbrido de páginas web (o sitios web) normales y una aplicación móvil. Este nuevo modelo de aplicación intenta combinar las características que ofrecen la mayoría de los navegadores modernos con los beneficios de la experiencia móvil.<br>
En 2015, la diseñadora Frances Berriman y el ingeniero de Google Chrome Alex Russell acuñaron el término "Aplicaciones web progresivas" para describir las aplicaciones que aprovechan las nuevas funciones compatibles con los navegadores modernos, incluidos Service Workers y Manifiestos de aplicaciones web, que permiten a los usuarios actualizar las aplicaciones web para ser aplicaciones de primera clase en su sistema operativo nativo.<br>
Según Google Developers, estas características son:<br>
- Progresivo: funciona para todos los usuarios, independientemente de la elección del navegador, ya que se construyeron con la mejora progresiva como principio fundamental.
- Capacidad de respuesta: se adapta a cualquier factor de forma: escritorio, dispositivo móvil, tableta o formularios que aún no han aparecido.
- Independiente de la conectividad: los trabajadores del servicio permiten trabajar sin conexión o en redes de baja calidad.
- Similar a una aplicación: siéntase como una aplicación para el usuario con interacciones y navegación al estilo de una aplicación.
- Fresco: siempre actualizado gracias al proceso de actualización del trabajador de servicio.
- Seguro: se sirve a través de HTTPS para evitar espionaje y garantizar que el contenido no haya sido manipulado.
- Descubribles: se pueden identificar como "aplicaciones" gracias a los manifiestos del W3C [6] y al alcance de registro del trabajador de servicios que permite a los motores de búsqueda encontrarlas.
- Re-interacción: facilite la re-interacción a través de funciones como notificaciones automáticas.
- Instalable: permite a los usuarios "conservar" las aplicaciones que encuentran más útiles en su pantalla de inicio sin la molestia de una tienda de aplicaciones.
- Vinculable: se comparte fácilmente a través de una URL y no requiere una instalación compleja.<br>  
<div class="source">- Wikipedia</div>

- Una guía para principiantes sobre aplicaciones web progresivas [leer]
- Aplicaciones web progresivas [leer]
- Introducción a las aplicaciones web progresivas [ver] [$]
- Creación de una aplicación web progresiva [ver] [$]
- Introducción a las aplicaciones web progresivas de Google [ver]
- Las aplicaciones nativas están condenadas [leer]
- Por qué las aplicaciones nativas están realmente condenadas: las aplicaciones nativas están condenadas pt 2 [leer]
- Tu primera aplicación web progresiva [leer]
- Aplicaciones web progresivas y sin conexión [ver] [$]

## 3.25 - Aprenda el diseño de API JS

- Diseñar mejores API de JavaScript [leer]
- Escribir API de JavaScript [leer]

## 3.26 - Aprenda las herramientas de desarrollo web del navegador

> Las herramientas de desarrollo web permiten a los desarrolladores web probar y depurar su código. Se diferencian de los creadores de sitios web y los IDE en que no ayudan en la creación directa de una página web, sino que son herramientas que se utilizan para probar la interfaz de usuario de un sitio web o aplicación web.<br>
Las herramientas de desarrollo web vienen como complementos del navegador o funciones integradas en los navegadores web. Los navegadores web más populares de la actualidad, como Google Chrome, Firefox, Opera, Internet Explorer y Safari, tienen herramientas integradas para ayudar a los desarrolladores web, y se pueden encontrar muchos complementos adicionales en sus respectivos centros de descarga de complementos.<br>
Las herramientas de desarrollo web permiten a los desarrolladores trabajar con una variedad de tecnologías web, incluidos HTML, CSS, DOM, JavaScript y otros componentes que maneja el navegador web. Debido a la creciente demanda de los navegadores web para hacer, los navegadores web más populares han incluido más funciones orientadas a los desarrolladores.<br>  
<div class="source">- Wikipedia</div>

Si bien la mayoría de los navegadores vienen equipados con herramientas de desarrollo web, las herramientas de desarrollo de Chrome son actualmente las más comentadas y utilizadas.

Sugeriría aprender y usar las herramientas de desarrollo web de Chrome, simplemente porque los mejores recursos para aprender herramientas de desarrollo web giran en torno a Chrome DevTools.

### Aprenda las herramientas para desarrolladores web de Chrome:

- Herramientas para desarrolladores de Chrome [ver] [$]
- Explore y domine las DevTools de Chrome [ver]
- Dominar las herramientas para desarrolladores de Chrome v2 [ver] [$]
- Uso de las herramientas para desarrolladores de Chrome [ver] [$]
- Aprender las herramientas para desarrolladores web de Chrome [ver] [$]

### Documentos de herramientas para desarrolladores web de Chrome:

- Referencia de la API de línea de comandos
- Referencia de accesos directos de teclado e interfaz de usuario
- Documentación por panel
- Configurar y personalizar DevTools

## 3.27 - Aprenda la línea de comandos (también conocida como CLI)

> Una interfaz de línea de comandos o un intérprete de lenguaje de comandos (CLI), también conocida como interfaz de usuario de línea de comandos, interfaz de usuario de consola e interfaz de usuario de caracteres (CUI), es un medio de interactuar con un programa de computadora cuando el usuario (o cliente) tiene problemas comandos al programa en forma de líneas sucesivas de texto (líneas de comando).<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- La guía de Bash [leer]
- Usuario avanzado de la línea de comandos [ver]
- Aprenda suficiente línea de comandos para ser peligroso [leer] [de gratis a $]

### Masterización:

- Técnicas avanzadas de línea de comandos [ver] [$]
- Introducción a Bash, VIM y Regex [ver] [$]

## 3.28 - Aprenda Node.js

> Node.js es un entorno de ejecución multiplataforma de código abierto para desarrollar aplicaciones web del lado del servidor. Las aplicaciones de Node.js están escritas en JavaScript y se pueden ejecutar dentro del tiempo de ejecución de Node.js en OS X, Microsoft Windows, Linux, FreeBSD, NonStop, IBM AIX, IBM System z e IBM i. Su trabajo está alojado y respaldado por Node.js Foundation, un proyecto colaborativo en Linux Foundation.<br> Node.js proporciona una arquitectura impulsada por eventos y una API de E/S sin bloqueo diseñada para optimizar el rendimiento y la escalabilidad de una aplicación en tiempo real. Utiliza el motor JavaScript Google V8 para ejecutar código y un gran porcentaje de los módulos básicos están escritos en JavaScript. Node.js contiene una biblioteca incorporada para permitir que las aplicaciones actúen como un servidor web sin software como Apache HTTP Server, Nginx o IIS.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- El arte de Node [leer]
- Introducción a Node.js [ver] [$]
- Introducción a Node.js de Evented Mind [ver]
- io.js y Node.js Siguiente: Primeros pasos [ver] [$]
- Aprendiendo Node: Pasar al lado del servidor [leer] [$]
- Learn You The Node.js [talleres autoguiados]
- Conceptos básicos de Node.js [ver] [$]
- Node.js en la práctica [leer] [$]
- Web en tiempo real con Node.js [ver]
- Diseño de API en Node.js, v3 [ver] [$]
- Aprenda Node [ver] [$]

## 3.29 - Aprenda módulos

### Aprendizaje general:

- JavaScript para programadores impacientes - Módulos [leer]
- Módulos ES6 en profundidad [leer]
- Explorando JS - Módulos [leer]
- Módulos ES: un análisis profundo de dibujos animados [leer]

### Referencias / Documentos:

- MDN - exportación
- MDN - importación

## 3.30 - Aprenda módulos cargadores/agrupadores

### Webpack:

- Webpack [leer]
- Conceptos básicos de Webpack 4 [ver] [$]
- Libro de paquete web de Survivejs.com [leer]

### Rollup:

- Rollup [leer]
  - Microbundle

### Parcel

- Parcel [leer]

## 3.31 - Aprenda administrador de paquetes

> Un administrador de paquetes o sistema de administración de paquetes es una colección de herramientas de software que automatiza el proceso de instalación, actualización, configuración y eliminación de paquetes de software para el sistema operativo de una computadora de manera consistente. Por lo general, mantiene una base de datos de dependencias de software e información de versión para evitar discrepancias de software y requisitos previos faltantes.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- Introducción a cómo funcionan los administradores de paquetes de JavaScript [leer]
- Los rangos de SemVer místicos y mágicos utilizados por npm & Bower [leer]
- Administradores de paquetes: una guía introductoria para el desarrollador front-end no iniciado [leer]
- Documentos sobre npm
- Documentos sobre yarn

## 3.32 - Aprenda control de versiones

> Un componente de la gestión de la configuración del software, el control de versiones, también conocido como control de revisión o control de fuente, es la gestión de cambios en documentos, programas informáticos, sitios web grandes y otras colecciones de información. Los cambios generalmente se identifican mediante un código numérico o de letras, denominado "número de revisión", "nivel de revisión" o simplemente "revisión". Por ejemplo, un conjunto inicial de archivos es "revisión 1". Cuando se realiza el primer cambio, el conjunto resultante es "revisión 2" y así sucesivamente. Cada revisión está asociada con una marca de tiempo y la persona que realiza el cambio. Las revisiones se pueden comparar, restaurar y combinar con algunos tipos de archivos.<br>  
<div class="source">- Wikipedia</div>

La solución más común utilizada hoy para el control de versiones es Git. ¡Aprenderlo!

### Aprendizaje general:

- Haciendo lo correcto [leer]
- Conceptos básicos de Git [ver] [$]
- Aprenda lo suficiente de Git [leer]
- Tutorial Git de Ry [leer]

### Masterización:

- Git en profundidad [ver] [$]
- Tutoriales avanzados de Git [leer]
- Pro Git [leer]
- Más información sobre la ramificación de Git [interactuar]

### Referencias / Documentos:

- https://git-scm.com/doc
- git-cheatsheet

## 3.33 - Aprenda la automatización de tareas y compilaciones

> La automatización de compilaciones es el proceso de automatizar la creación de una compilación de software y los procesos asociados que incluyen: compilar el código fuente de la computadora en código binario, empaquetar código binario y ejecutar pruebas automatizadas.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- Introducción a Gulp [leer] [$]
- Conceptos básicos de Gulp [ver] [$]
- Automatización de compilación de JavaScript con Gulp.js [ver] [$]

### Referencias / Documentos:

- Gulp

Gulp es genial. Sin embargo, es posible que solo necesite ejecutar npm. Antes de pasar a la complejidad adicional en su pila de aplicaciones, pregúntese si npm run puede hacer el trabajo. Si necesitas más, usa Gulp.

Lee:

- ¡Dale la Boot a Grunt! Una guía para usar npm como herramienta de compilación
- Usando npm como un sistema de compilación para su próximo proyecto
- Uso de npm como Task Runner [ver] [$]
- Por qué dejé Gulp y Grunt por scripts npm
- ¿Por qué npm Scripts?

## 3.34 - Aprenda sobre la optimización del rendimiento del sitio

> La optimización del rendimiento web, WPO u optimización del sitio web es el campo de conocimiento sobre cómo aumentar la velocidad en la que las páginas web se descargan y se muestran en el navegador web del usuario. Dado que la velocidad promedio de Internet aumenta a nivel mundial, es apropiado que los administradores de sitios web y los webmasters consideren el tiempo que tardan los sitios web en mostrarse para el visitante.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- Optimización de la representación del navegador [ver]
- Sitios web aún más rápidos: mejores prácticas de rendimiento para desarrolladores web [leer] [$]
- Sitios web de alto rendimiento: conocimientos esenciales para los ingenieros de front-end [leer] [$]
- El rendimiento de JavaScript sobresale [leer] [$]
- Reglas de PageSpeed ​​Insights [leer]
- perf-tooling.today [leer]
- Calendario de rendimiento [leer]
- perf.rocks [leer]
- Usando WebPageTest [leer] [$]
- Libro diario de rendimiento web, volumen 2 [leer] [$]
- Rendimiento del sitio web [ver] [$]
- Rendimiento web con Webpack 4 [ver] [$]
- Optimización del rendimiento del sitio web [ver]
- Lista de verificación de rendimiento de front-end 2019 [PDF, páginas de Apple, MS Word] [leer]

## 3.35 - Aprenda a realizar pruebas

> **Pruebas unitarias**: en programación de computadoras, las pruebas unitarias son un método de prueba de software mediante el cual unidades individuales de código fuente, conjuntos de uno o más módulos de programas de computadora junto con el control asociado
Los datos, los procedimientos de uso y los procedimientos operativos se prueban para determinar si son aptos para su uso. Intuitivamente, uno puede ver una unidad como la parte más pequeña que se puede probar de una aplicación.<br>  
<div class="source">- Wikipedia</div>

> **Pruebas funcionales**: las pruebas funcionales son un proceso de garantía de calidad (QA) y un tipo de prueba de caja negra que basa sus casos de prueba en las especificaciones del componente de software bajo prueba. Las funciones se prueban alimentándolas de entrada y examinando la salida, y la estructura interna del programa rara vez se considera (no como en las pruebas de caja blanca). Las pruebas funcionales generalmente describen lo que hace el sistema.<br>  
<div class="source">- Wikipedia</div>

> **Pruebas de integración**: las pruebas de integración (a veces llamadas integración y pruebas, abreviado I&T) es la fase de las pruebas de software en la que los módulos de software individuales se combinan y prueban como un grupo. Ocurre después de las pruebas unitarias y antes de las pruebas de validación. La prueba de integración toma como entrada los módulos que han sido probados por unidad, los agrupa en agregados más grandes, aplica las pruebas definidas en un plan de prueba de integración a esos agregados y entrega como salida el sistema integrado listo para la prueba del sistema.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- Principios y prácticas de prueba de JavaScript [ver] [$]
- Primero, el front-end: prueba y creación de prototipos de aplicaciones JavaScript [ver] [$]
- Let's Code: JavaScript basado en pruebas [ver] [$]
- Prueba de JavaScript [ver]
- Recetas de prueba de JavaScript [leer] [$]
- JavaScript comprobable [leer] [$]
- Pruebas de aplicaciones de JavaScript: código rápido, seguro y que se puede mantener [leer] [$]
- Desarrollo de JavaScript basado en pruebas [leer] [$]
- The Way of the Web Tester: Guía para principiantes sobre la automatización de pruebas [leer] [$]
- Prueba de aplicaciones React, v2 [ver] [$]
- Aprenda las pruebas unitarias de JavaScript con Mocha, Chai y Sinon [ver] [$]

## 3.36 - Aprenda los navegadores sin cabeza

> Un navegador sin cabeza es un navegador web sin una interfaz gráfica de usuario.<br>
Los navegadores sin cabeza proporcionan control automatizado de una página web en un entorno similar a los navegadores web populares, pero se ejecutan a través de una interfaz de línea de comandos o mediante la comunicación de red. Son particularmente útiles para probar páginas web, ya que pueden representar y comprender HTML de la misma manera que lo haría un navegador, incluidos elementos de estilo como diseño de página, color, selección de fuentes y ejecución de JavaScript y AJAX que generalmente no están disponibles cuando se usa otros métodos de prueba. Google declaró en 2009 que el uso de un navegador sin cabeza podría ayudar a su motor de búsqueda a indexar el contenido de los sitios web que usan AJAX.<br>  
<div class="source">- Wikipedia</div>

- Introducción a Headless Chrome [léame]

PhantomJS ya no se mantiene, Headless Chrome interviene.

## 3.37 - Aprenda desarrollo sin conexión

El desarrollo fuera de línea (también conocido como fuera de línea primero) es un área de conocimiento y discusión en torno a las prácticas de desarrollo para dispositivos que no siempre están conectados a Internet o a una fuente de alimentación.

### Aprendizaje general:

- Creación de aplicaciones web HTML5 sin conexión [leer]
- Todo lo que necesita saber para crear aplicaciones web sin conexión primero [leer]
- Sin conexión primero [leer]
- offlinefirst.org [leer]
- El libro de cocina sin conexión [leer]
- Inicio rápido sin conexión [leer]

## 3.38 - Aprenda seguridad web / navegador / aplicación

- Manual de seguridad del navegador [leer]
- Seguridad frontend [ver]
- Hacksplaining [leer]
- Hoja de referencia de seguridad HTML5 [leer]
- Prácticas recomendadas de seguridad HTTP [leer]
- Seguridad de identidad y datos para el desarrollo web: prácticas recomendadas leer
Seguridad para desarrolladores web: uso de JavaScript, HTML y CSS [leer] [$]
- Conceptos básicos de la seguridad de las aplicaciones web [leer]
- Internet: cifrado y claves públicas [ver]
- Internet: ciberseguridad y delitos [ver]
- The Tangled Web: Una guía para proteger las aplicaciones web modernas [leer] [$]
- Conceptos básicos de seguridad web [leer]
- Seguridad web [leer]
- Seguridad web [ver] [$]
- Pila completa para ingenieros de front-end [ver] [$]

## 3.39 - Aprenda el desarrollo multidispositivo

![Esto será la web](/courses/front-end-developer-handbook-2019/chapter3-8.png)

<div class="source">Fuente de la imagen: http://bradfrost.com/blog/post/this-is-the-web/</div>

Un sitio web o una aplicación web puede ejecutarse en una amplia gama de computadoras, portátiles, tabletas y teléfonos, así como en un puñado de dispositivos nuevos (relojes, termostatos, refrigeradores, etc.). La forma en que determina qué dispositivos admitirá y cómo desarrollará para admitir esos dispositivos se denomina "estrategia de desarrollo de dispositivos múltiples". A continuación, enumero las estrategias de desarrollo multidispositivo más comunes.

- Cree un sitio web / aplicación con capacidad de respuesta (RWD) para todos los dispositivos.
- Cree un sitio web / aplicación adaptable / progresivamente mejorado para todos los dispositivos.
- Cree un sitio web, una aplicación web, una aplicación nativa o una aplicación nativa híbrida para cada dispositivo individual o grupo de dispositivos.
- Intente modernizar algo que ya ha construido utilizando bits y partes de las estrategias 1, 2 o 3.

### Aprendizaje general:

- Un libro Apart Pack - Diseño web adaptable [leer] [$]
- Un paquete de libro aparte: diseño para cualquier dispositivo [leer] [$]
- Diseño web adaptable [leer] [$]
- Diseñar con mejora progresiva [leer] [$]
- Desarrollo web móvil [ver]
- CSS Grids y Flexbox para diseño web adaptable [ver] [$]
- Diseño de correo electrónico HTML receptivo [ver] [$]
- Imágenes receptivas [ver]
- Tipografía web adaptable, v2 [ver] [$]
- Conceptos básicos del diseño web adaptable [ver]
