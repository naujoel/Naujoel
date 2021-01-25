---
title: Capítulo 3. Aprendizaje del desarrollador front-end. Recursos (recomendaciones) autodirigidos
linktitle: Capítulo 3. Aprendizaje del desarrollador front-end. Recursos (recomendaciones) autodirigidos
toc: true
type: docs
date: "2020-09-04T00:00:00+01:00"
draft: true
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

- [¿Que es la Internet?](https://www.youtube.com/watch?v=Dxcc6ycZ73M) [ver]
- [Conceptos básicos de Internet](http://internetfundamentals.com/) [ver]
- [Cómo funciona la Web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works) [leer]
- ¿Cómo funciona el internet? https://developer.mozilla.org/en-US/docs/Learn/Common_questions/How_does_the_Internet_work y http://web.stanford.edu/class/msande91si/www-spr04/readings/week1/InternetWhitepaper.htm [leer]
- [Cómo funciona Internet](https://www.khanacademy.org/partner-content/code-org/internet-works) [ver]
- [Cómo funciona Internet en 5 minutos](https://www.youtube.com/watch?v=7_LPdttKXPc) [ver]
- [Cómo funciona la Web](https://www.eventedmind.com/classes/how-the-web-works-7f40254c) [ver]
- [¿Que es la Internet? O, "Tú dices tomate, yo digo TCP/IP"](http://www.20thingsilearned.com/en-US/what-is-the-internet/1) [leer]
- [No temas a Internet](http://www.dontfeartheinternet.com/)

![Quién ejecuta internet](/courses/front-end-developer-handbook-2019/chapter3-2.png)

<div class="source">Fuente de la imagen: http://www.bitrebels.com/technology/find-out-who-runs-the-internet-chart/</div>

## 3.2. - Aprender navegadores web

> Un navegador web (comúnmente conocido como navegador) es una aplicación de software para recuperar, presentar y recorrer recursos de información en la World Wide Web. Un recurso de información se identifica mediante un Identificador de recurso uniforme (URI / URL) y puede ser una página web, una imagen, un video u otro contenido. Los hipervínculos presentes en los recursos permiten a los usuarios navegar fácilmente en sus navegadores hacia los recursos relacionados. Aunque los navegadores están diseñados principalmente para usar la World Wide Web, también se pueden usar para acceder a información proporcionada por servidores web en redes privadas o archivos en sistemas de archivos.<br>  
<div class="source">-Wikipedia</div>

Los [navegadores más utilizados](https://netmarketshare.com/?options=%7B%22filter%22%3A%7B%22%24and%22%3A%5B%7B%22deviceType%22%3A%7B%22%24in%22%3A%5B%22Desktop%2Flaptop%22%2C%22Mobile%22%5D%7D%7D%5D%7D%2C%22dateLabel%22%3A%22Trend%22%2C%22attributes%22%3A%22share%22%2C%22group%22%3A%22browser%22%2C%22sort%22%3A%7B%22share%22%3A-1%7D%2C%22id%22%3A%22browsersDesktop%22%2C%22dateInterval%22%3A%22Monthly%22%2C%22dateStart%22%3A%222018-01%22%2C%22dateEnd%22%3A%222018-12%22%2C%22segments%22%3A%22-1000%22%7D) (en computadoras de escritorio y móviles) son:

1. [Chrome](http://www.google.com/chrome/) (motor: [Blink](https://en.wikipedia.org/wiki/Blink_%28layout_engine%29) + [V8](https://en.wikipedia.org/wiki/V8_%28JavaScript_engine%29))
2. [Firefox](https://www.mozilla.org/en-US/firefox/new/) (motor: [Gecko](https://en.wikipedia.org/wiki/Gecko_%28software%29) + [SpiderMonkey](https://en.wikipedia.org/wiki/SpiderMonkey_%28software%29))
3. [Internet Explorer](http://windows.microsoft.com/en-us/internet-explorer/download-ie) (motor: [Trident](https://en.wikipedia.org/wiki/Trident_%28layout_engine%29) + [Chakra](https://en.wikipedia.org/wiki/Chakra_%28JScript_engine%29))
4. [Safari](https://www.apple.com/safari/) (motor: [Webkit](https://en.wikipedia.org/wiki/WebKit) + [SquirrelFish](https://trac.webkit.org/wiki/SquirrelFish))

![Porcentaje de uso de navegadores](/courses/front-end-developer-handbook-2019/chapter3-3.png)

<div class="source">Fuente de la imagen: http://gs.statcounter.com/browser-market-share</div>

### Evolución de los navegadores y las tecnologías web (es decir, API)

- [evolutionoftheweb.com](http://www.evolutionoftheweb.com/) [leer]
- [Cronología de los navegadores web](https://en.wikipedia.org/wiki/Timeline_of_web_browsers) [leer]

### Los [navegadores sin cabeza](http://www.asad.pw/HeadlessBrowsers/) más utilizados son:

- [Chromium sin cabeza](https://chromium.googlesource.com/chromium/src/+/lkgr/headless/README.md) (motor: [Blink](https://www.chromium.org/blink) + V8)
- [SlimerJS](http://slimerjs.org/) (motor: [Gecko](https://en.wikipedia.org/wiki/Gecko_%28software%29) + [SpiderMonkey](https://en.wikipedia.org/wiki/SpiderMonkey_%28software%29))

### Cómo funcionan los navegadores

- [20 cosas que aprendí sobre los navegadores y la Web](http://www.20thingsilearned.com/en-US/foreword/1) [leer]
- [CSS rápido: cómo diseñan los navegadores las páginas web](http://dbaron.org/talks/2012-03-11-sxsw/master.xhtml) [leer]
- [Cómo funcionan los navegadores: entre bastidores de los navegadores web modernos](http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/) [leer]
- [Quantum Up Close: ¿Qué es un motor de navegador?](https://hacks.mozilla.org/2017/05/quantum-up-close-what-is-a-browser-engine/)
- [Entonces, ¿cómo procesa realmente el navegador un sitio web?](https://www.youtube.com/watch?v=SmE4OwHztCc) [Ver]
- [Qué fuerza el diseño / reflujo](https://gist.github.com/paulirish/5d52fb081b3570c81e3a) [leer]
- [Lo que todo desarrollador de frontend debe saber sobre el renderizado de páginas web](http://frontendbabel.info/articles/webpage-rendering-101/) [leer]

### Optimización para navegadores:

- [Optimización de la representación del navegador](https://www.udacity.com/course/browser-rendering-optimization--ud860) [ver]
- [Optimización del rendimiento del sitio web](https://www.udacity.com/course/website-performance-optimization--ud884) [ver]

### Comparación de navegadores

- [Comparación de navegadores web](https://en.wikipedia.org/wiki/Comparison_of_web_browsers) [leer]

### Hacks del navegador

- [browserhacks.com](http://browserhacks.com/) [leer]

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

- [Introducción a la terminología, los componentes y los conceptos de DNS](https://www.digitalocean.com/community/tutorials/an-introduction-to-dns-terminology-components-and-concepts) [leer]
- [DNS explicado](https://www.youtube.com/watch?v=72snZctFFtA) [ver]
- [Cómo funciona el DNS](https://howdns.works/ep1/) [leer]
- [Internet: direcciones IP y DNS](https://www.youtube.com/watch?v=5o8CwafCxnU&index=3&list=PLzdnOPI1iJNfMRZm5DDxco3UdsFegvuB7) [ver]
- [¿Qué es un nombre de dominio?](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_domain_name) [leer]

## 3.4 - Aprenda HTTP / Redes (incluidos CORS y WebSockets)

> **HTTP**: el protocolo de transferencia de hipertexto (HTTP) es un protocolo de aplicación para sistemas de información hipermedia distribuidos y colaborativos. HTTP es la base de la comunicación de datos para la World Wide Web.<br>  
<div class="source">- Wikipedia</div>

### Especificaciones HTTP

- [HTTP/2](https://http2.github.io/)
- [Protocolo de transferencia de hipertexto - HTTP/1.1](https://tools.ietf.org/html/rfc2616)

### Documentos HTTP

- [MDN HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP) [leer]

### Vídeos / artículos / tutoriales de HTTP

- [Redes de navegadores de alto rendimiento: lo que todo desarrollador web debe saber acerca de las redes y el rendimiento web](http://chimera.labs.oreilly.com/books/1230000000545/index.html) [leer]
- [MDN: descripción general de HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview) [leer]
- [HTTP: La guía definitiva](https://www.amazon.com/HTTP-Definitive-Guide-Guides/dp/1565925092/ref=cm_cr_arp_d_product_top?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=11b990b79d33ddbef63712765715a9c1&camp=1789&creative=9325) (Guías definitivas) [leer] [$]
- [Preguntas frecuentes sobre HTTP/2](https://http2.github.io/faq/#what-are-the-key-differences-to-http1x) [leer]
- [Conceptos básicos de HTTP](http://www.pluralsight.com/courses/xhttp-fund) [ver] [$]
- [Conceptos básicos de HTTP/2](https://app.pluralsight.com/library/courses/http2-fundamentals/table-of-contents) [ver] [$]
- [HTTP: el protocolo que todo desarrollador web debe conocer - Parte 1](http://code.tutsplus.com/tutorials/http-the-protocol-every-web-developer-must-know-part-1--net-31177) [leer]
- [HTTP: el protocolo que todo desarrollador web debe conocer - Parte 2](http://code.tutsplus.com/tutorials/http-the-protocol-every-web-developer-must-know-part-2--net-31155) [leer]
- [HTTP sucintamente](http://code.tutsplus.com/series/http-succinctly--net-33683) [leer]

### Códigos de estado HTTP

- [Códigos de estado HTTP](https://httpstatuses.com/)
- [Códigos de estado HTTP en 60 segundos](http://webdesign.tutsplus.com/tutorials/http-status-codes-in-60-seconds--cms-24317) [ver]

> **CORS**: el intercambio de recursos de origen cruzado (CORS) es un mecanismo que permite solicitar recursos restringidos (por ejemplo, fuentes) en una página web desde otro dominio fuera del dominio desde el que se originó el recurso.<br>  
<div class="source">- Wikipedia</div>

### Especificaciones CORS

- [Uso compartido de recursos entre orígenes](https://www.w3.org/TR/cors/)

### CORS

- [CORS en acción](https://www.amazon.com/CORS-Action-Creating-consuming-cross-origin/dp/161729182X/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=47ebd885d688a4ed69f77a1bd8273f8a&camp=1789&creative=9325) [leer] [$]
- [Control de acceso HTTP (CORS)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Access_control_CORS) [leer]

> **WebSockets**: WebSocket es un protocolo que proporciona canales de comunicación full-duplex a través de una sola conexión TCP. El protocolo WebSocket fue estandarizado por IETF como RFC 6455 en 2011, y la API WebSocket en Web IDL está siendo estandarizada por el W3C.<br>  
<div class="source">- Wikipedia</div>

### WebSockets

- [Conecta la Web con WebSockets](https://code.tutsplus.com/courses/connect-the-web-with-websockets) [ver]
- [WebSocket: Comunicaciones ligeras cliente-servidor](https://www.amazon.com/WebSocket-Client-Server-Communications-Andrew-Lombardi/dp/1449369278/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=dd39395cf3d2ab4fc7c820d7c19db39a&camp=1789&creative=9325) [leer] [$]
- [El protocolo WebSocket](https://tools.ietf.org/html/rfc6455) [leer]

## 3.5 - Aprenda alojamiento web

> Un servicio de alojamiento web es un tipo de servicio de alojamiento de Internet que permite a las personas y organizaciones hacer que su sitio web sea accesible a través de la World Wide Web. Los servidores web son empresas que proporcionan espacio en un servidor de propiedad o alquilado para su uso por los clientes, además de proporcionar conectividad a Internet, normalmente en un centro de datos.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- [Alojamiento web 101: Obtenga su sitio web en vivo en la Web en muy poco tiempo](https://www.udemy.com/web-hosting-101/) [video]

![Qué es web hosting](/courses/front-end-developer-handbook-2019/chapter3-5.png)

<div class="source">Fuente de la imagen: https://firstsiteguide.com/wp-content/uploads/2016/06/what-is-web-hosting-infographic.jpg</div>

## 3.6 - Aprenda el desarrollo general de front-end

- [Frontend Bootcamp/Days in the Web](https://github.com/Microsoft/frontend-bootcamp) [leer]
- [Convertirse en un desarrollador web preparado para una carrera](https://frontendmasters.com/learn/beginner/)
- [Conviértase en desarrollador web front-end](https://www.lynda.com/learning-paths/Web/become-a-front-end-web-developer) [ver] [$]
- [Ser desarrollador web](http://www.yellowshoe.com.au/standards) [leer]
- [freeCodeCamp](http://freecodecamp.com/) [interactuar]
  - [aprender el desarrollo de front-end durante #100DaysOfCode](https://github.com/nas5w/100-days-of-code-frontend#contibuting) [leer]
- [Nanodegree de desarrollador web front-end](https://www.udacity.com/course/front-end-web-developer-nanodegree--nd001) [ver] [$]
- [Inicio de carrera en desarrollo web front-end](http://www.pluralsight.com/courses/front-end-web-development-career-kickstart) [ver] [$]
- [Desarrollo web front-end: empezar](http://www.pluralsight.com/courses/front-end-web-development-get-started) [ver] [$]
- [Inicio rápido del desarrollo web front-end con HTML5, CSS y JavaScript](http://www.pluralsight.com/courses/front-end-web-app-html5-javascript-css) [ver] [$]
- [Desarrollo web front-end: la guía de Big Nerd Ranch](https://www.amazon.com/Front-End-Web-Development-Ranch-Guide/dp/0134433947/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=06802d4e42ca55b03294779c960d0826&camp=1789&creative=9325) [leer] [$]
- [Introducción completa al desarrollo web](https://frontendmasters.com/courses/web-development-v2/) [ver] [$]
- [Más información sobre desarrollo web front-end](https://teamtreehouse.com/tracks/front-end-web-development) [ver] [$]
- [Entonces, desea ser un ingeniero de aplicaciones para el usuario](https://www.youtube.com/watch?v=Lsg84NtJbmI) [ver]
- [codecademy.com: Ruta de desarrollo web](https://www.codecademy.com/learn/paths/web-development) [interactuar] [de gratis a $]
- [web.dev](https://web.dev/learn) [leer]

## 3.7 - Aprenda diseño de interacción/interfaz de usuario

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

- [Acerca de la cara: lo esencial del diseño de interacción](https://www.amazon.com/About-Face-Essentials-Interaction-Design-ebook/dp/B00MFPZ9UY/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=c723c84ad4d246cb7f1c4a737c5f38a4&camp=1789&creative=9325) [leer] [$]
- [Diseño para piratas informáticos: belleza de ingeniería inversa](https://www.amazon.com/Design-Hackers-Reverse-Engineering-Beauty/dp/1119998956/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=2a52f0968de21c03f069d857b9d92b37&camp=1789&creative=9325) [leer] [$]
- [Diseño para no diseñadores](https://www.youtube.com/watch?v=ZbrzdMaumNk&feature=youtu.be) [ver]
- [Diseño de interfaces](https://www.amazon.com/Designing-Interfaces-Jenifer-Tidwell/dp/1449379702/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=4539707bb145c676472472aab25eaa56&camp=1789&creative=9325) [leer] [$]
- [Diseño de interfaces web: principios y patrones para interacciones enriquecidas](https://www.amazon.com/Designing-Web-Interfaces-Principles-Interactions-ebook/dp/B0026OR33U/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=03fb59f4a4345732fae9ecdfaa5076ae&camp=1789&creative=9325) [leer] [$]
- [Don't Make Me Think, Revisited: Un enfoque de sentido común para la usabilidad web](https://www.amazon.com/Dont-Make-Think-Revisited-Usability/dp/0321965515/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=8b0b0771a9985e4e030ef1fe29cf6409&camp=1789&creative=9325) [leer] [$]

## 3.8 - Aprenda HTML y CSS

> **HTML**: el lenguaje de marcado de hipertexto, comúnmente conocido como HTML, es el lenguaje de marcado estándar que se utiliza para crear páginas web. Los navegadores web pueden leer archivos HTML y convertirlos en páginas web visibles o audibles. HTML describe la estructura de un sitio web semánticamente junto con pistas para la presentación, lo que lo convierte en un lenguaje de marcado, en lugar de un lenguaje de programación.<br>  
<div class="source">- Wikipedia</div>

> **CSS**: hojas de estilo en cascada (CSS) es un lenguaje de hojas de estilo que se utiliza para describir el aspecto y el formato de un documento escrito en un lenguaje de marcado. Aunque se utiliza con mayor frecuencia para cambiar el estilo de las páginas web y las interfaces de usuario escritas en HTML y XHTML, el lenguaje se puede aplicar a cualquier tipo de documento XML, incluidos XML simple, SVG y XUL. Junto con HTML y JavaScript, CSS es una tecnología fundamental utilizada por la mayoría de los sitios web para crear páginas web visualmente atractivas, interfaces de usuario para aplicaciones web e interfaces de usuario para muchas aplicaciones móviles.<br>  
<div class="source">- Wikipedia</div>

Al igual que con la construcción de una casa, se podría considerar HTML como marco y CSS como pintura y decoración.

### Aprendizaje general:

- [Centrado absoluto en CSS](http://codepen.io/shshaw/full/gEiDt) [leer]
- [Posicionamiento CSS](http://www.pluralsight.com/courses/css-positioning-1834) [ver] [$]
- [Introducción al desarrollo web (v2)](https://frontendmasters.com/courses/web-development-v2/) [ver] [$]
- [Desarrollo web front-end: comenzar](http://www.pluralsight.com/courses/front-end-web-development-get-started) [ver] [$]
- [Inicio rápido del desarrollo web front-end con HTML5, CSS y JavaScript](http://www.pluralsight.com/courses/front-end-web-app-html5-javascript-css) [ver] [$]
- [HTML y CSS: diseño y creación de sitios web](https://www.amazon.com/gp/product/1118008189/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=b1c45ab715f267f7dfed8c981c14eceb&camp=1789&creative=9325) [leer] [$]
- [Flujo de documentos HTML](http://www.pluralsight.com/courses/html-document-flow-1837) [ver] [$]
- [Dominio de HTML: semántica, estándares y estilo](https://www.amazon.com/gp/product/1590597656/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=a5c4eb997239ea9e57a86456cef7763c&camp=1789&creative=9325) [leer] [$]
- [Interneting es difícil](https://internetingishard.com/) [leer]
- [Introducción a HTML/CSS: creación de páginas web](https://www.khanacademy.org/computing/computer-programming/html-css) [ver]
- [Aprenda a codificar HTML y CSS](http://learn.shayhowe.com/html-css/) [leer]
- [Aprenda el diseño CSS](http://learnlayout.com/) [leer]
- [MarkSheet](http://marksheet.io/) [leer]
- [MDN: HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML) [leer]
- [MDN: CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS) [leer]
- [HTML semántico: cómo estructurar páginas web](https://webdesign.tutsplus.com/courses/semantic-html-how-to-structure-web-pages) [ver]
- [Estructura sólida de formulario HTML](https://webdesign.tutsplus.com/courses/solid-html-form-structure) [ver]
- [Comprensión del modelo de caja CSS](https://webdesign.tutsplus.com/courses/understanding-the-css-box-model) [ver]
- [Diseño web resiliente](https://resilientwebdesign.com/) [leer]

### Dominar CSS:

- [Una guía completa de Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) [leer]
- [CSS Grids y Flexbox para diseño web adaptable](https://frontendmasters.com/courses/css-grids-flexbox/) [ver] [$]
- [CSS Diner](http://flukeout.github.io/) [interactuar]
- [Selectores de CSS desde CSS4 hasta CSS1](http://css4-selectors.com/selectors/) [leer]
- [Secretos de CSS: mejores soluciones para los problemas cotidianos de diseño web](https://www.amazon.com/CSS-Secrets-Solutions-Everyday-Problems/dp/1449372635/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=40a9480c18839b4b2ea798aa2afafd0e&camp=1789&creative=9325) [leer] [$]
- [CSS3](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS3) [leer]
- [CSS en profundidad, v2](https://frontendmasters.com/courses/css-in-depth-v2/) [ver] [$]
- [¿Qué es el Flexbox? Un curso de 20 videos simple y gratuito que lo ayudará a dominar CSS y
Flexbox](http://flexbox.io/) [ver]
- [30 Seconds of CSS: una colección cuidada de fragmentos de CSS útiles que puede comprender en 30 segundos o menos.](https://atomiks.github.io/30-seconds-of-css/) [leer]

### Referencias / Documentos:

- [CSS Triggers ... un juego de diseño, pintura y composición](http://csstriggers.com/)
- [cssreference.io](http://cssreference.io/)
- [cssvalues.com](http://cssvalues.com/)
- [CSS predeterminado para el navegador Chrome](https://chromium.googlesource.com/chromium/blink/+/master/Source/core/css/html.css)
- [Head: una lista de todo lo que podría incluirse en el head de tu documento](http://gethead.info/)
- [Referencia de atributos HTML](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes)
- [Referencia CSS de MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)
- [Referencia de elementos HTML de MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

### Glosario / Vocabulario:

- [Glosario de CSS: referencia de programación para comentarios, propiedades y selectores de cobertura de CSS](https://www.codecademy.com/articles/glossary-css)
- [Vocabulario CSS](http://apps.workflower.fi/vocabs/css/en)
- [Referencia de programación del glosario HTML para elementos HTML](https://www.codecademy.com/articles/glossary-html)

### Estándares / Especificaciones:

- [Todas las especificaciones CSS del W3C](http://www.w3.org/Style/CSS/current-work#roadmap)
- [Todas las especificaciones HTML del W3C](http://www.w3.org/standards/techs/html#w3c_all)
- [Especificación de hojas de estilo en cascada Nivel 2 Revisión 2 (CSS 2.2)](https://drafts.csswg.org/css2/)
- [Índices CSS: una lista de todos los términos definidos por las especificaciones CSS](https://drafts.csswg.org/indexes/)
- [Los elementos de HTML del estándar de vida](https://html.spec.whatwg.org/multipage/semantics.html#semantics)
- [Atributos globales](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes)
- La [sintaxis HTML](https://html.spec.whatwg.org/multipage/syntax.html#syntax) de Living Standard
- [HTML 5.2 de W3C](http://w3c.github.io/html/)
- [Selectores Nivel 3](http://www.w3.org/TR/css3-selectors/)

### Arquitectura de CSS:

- [Diseño atómico](http://atomicdesign.bradfrost.com/) [leer]
- [BEM](http://getbem.com/introduction/)
- [ITCSS](https://www.xfive.co/blog/itcss-scalable-maintainable-css-architecture/)
- [OOCSS](http://oocss.org/) [leer]
- [SMACSS](https://smacss.com/) [leer] [$]
  - [Arquitectura modular escalable para CSS (SMACSS)](https://frontendmasters.com/courses/smacss/) [ver] [$]
- [SUIT CSS](http://suitcss.github.io/)
- [rscss](http://rscss.io/)

### Convenciones de autoría / arquitectura:

- [Guía de código CSS](http://codeguide.co/#css) [leer]
- [css-arquitectura](https://github.com/jareware/css-architecture)
- [cssguidelin.es](http://cssguidelin.es/) [leer]
- [CSS idiomático](https://github.com/necolas/idiomatic-css) [leer]
- [MaintainableCSS](http://maintainablecss.com/) [leer]
- [Estándares para desarrollar HTML y CSS flexibles, duraderos y sostenibles](http://mdo.github.io/code-guide/) [leer]

## 3.9 - Aprenda la optimización de motores de búsqueda

> La optimización de motores de búsqueda (SEO) es el proceso de afectar la visibilidad de un sitio web o una página web en los resultados no pagados de un motor de búsqueda, a menudo denominados resultados "naturales", "orgánicos" o "obtenidos". En general, cuanto más temprano (o mejor clasificado en la página de resultados de búsqueda), y con más frecuencia aparezca un sitio en la lista de resultados de búsqueda, más visitantes recibirá de los usuarios del motor de búsqueda. El SEO puede apuntar a diferentes tipos de búsqueda, incluida la búsqueda de imágenes, la búsqueda local, la búsqueda de videos, la búsqueda académica, la búsqueda de noticias y los motores de búsqueda verticales específicos de la industria.<br>  
<div class="source">- Wikipedia</div>

![SEO explicado](/courses/front-end-developer-handbook-2019/chapter3-6.png)

<div class="source">Fuente de la imagen: https://visual.ly/community/infographic/computers/how-does-seo-work</div>

### Aprendizaje general:

- [Guía de inicio de optimización de motores de búsqueda de Google](http://static.googleusercontent.com/media/www.google.com/en//webmasters/docs/search-engine-optimization-starter-guide.pdf) [leer]
- [SEO moderno](https://frontendmasters.com/courses/modern-seo/) [ver] [$]
- [Conceptos básicos de SEO de David Booth](http://www.lynda.com/Analytics-tutorials/SEO-Fundamentals/187858-2.html) [ver] [$]
- [Conceptos básicos de SEO de Paul Wilson](http://www.pluralsight.com/courses/seo-fundamentals) [ver] [$]
- [Tutorial de SEO para principiantes en 2016](http://www.hobo-web.co.uk/seo-tutorial/) [leer]
- [SEO para diseñadores web](https://webdesign.tutsplus.com/courses/seo-for-web-designers) [ver] [$]

## 3.10 - Aprenda JavaScript

> JavaScript es un lenguaje de programación de alto nivel, dinámico, sin tipo e interpretado. Se ha estandarizado en la especificación del lenguaje ECMAScript. Junto con HTML y CSS, es una de las tres tecnologías esenciales de la producción de contenido en la World Wide Web; la mayoría de los sitios web lo utilizan y es compatible con todos los navegadores web modernos sin complementos. JavaScript está basado en prototipos con funciones de primera clase, lo que lo convierte en un lenguaje de múltiples paradigmas, que admite estilos de programación orientados a objetos, imperativos y funcionales. Tiene una API para trabajar con texto, matrices, fechas y expresiones regulares, pero no incluye ninguna E / S, como redes, almacenamiento o instalaciones de gráficos, confiando para estos en el entorno host en el que está integrado.<br>  
<div class="source">- Wikipedia</div>

### Empezando:

- [MDN: JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript) [leer]
- [javascript.info](http://javascript.info/)
- [Ilustración de JavaScript](http://www.javascriptenlightenment.com/) [leer]
- [JavaScript elocuente](http://eloquentjavascript.net/) [leer]

### Aprendizaje general:

- [Hablando JavaScript](http://speakingjs.com/es5/index.html) [leer]
- [JavaScript para programadores impacientes](http://exploringjs.com/impatient-js/index.html) [leer]
- [No conoces JS: Up & Going](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20&%20going/README.md#you-dont-know-js-up--going) [leer]
- [No conoces JS: tipos y gramática](https://github.com/getify/You-Dont-Know-JS/blob/master/types%20&%20grammar/README.md#you-dont-know-js-types--grammar) [leer]
- [No conoces JS: alcance y cierres](https://github.com/getify/You-Dont-Know-JS/blob/master/scope%20&%20closures/README.md#you-dont-know-js-scope--closures) [leer]
- [No conoces JS: this y prototipos de objetos](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20&%20object%20prototypes/README.md#you-dont-know-js-this--object-prototypes) [leer]
- [Hoja de referencia de JavaScript moderna: hoja de referencia para JavaScript, conocimiento que encontrará con frecuencia en proyectos modernos.](https://github.com/mbeaudru/modern-js-cheatsheet) [leer]
- [JavaScript: Las partes difíciles](https://frontendmasters.com/courses/javascript-hard-parts/) [ver] [$]
- [Fundamentos profundos de JavaScript (v3)](https://frontendmasters.com/courses/deep-javascript-v3/) [ver] [$]

### Masterización:

- [Configuración de ES6](https://leanpub.com/setting-up-es6) [leer]
- [ES6 PARA TODOS!](https://es6.io/) [ver] [$]
- [Explorando ES6](http://exploringjs.com/es6.html) [leer]
- [No conoces JS: ES6 y más allá](https://github.com/getify/You-Dont-Know-JS/blob/master/es6%20&%20beyond/README.md#you-dont-know-js-es6--beyond) [leer]
- [Comprensión de ECMAScript 6: la guía definitiva para desarrolladores de JavaScript](https://www.amazon.com/Understanding-ECMAScript-Definitive-JavaScript-Developers/dp/1593277571/ref=as_li_ss_tl?&_encoding=UTF8&tag=fronenddevejo-20&linkCode=ur2&linkId=1ca4f5f23b42aeadad0990ab3bf91ca7&camp=1789&creative=9325) [leer] [$]
- [JavaScript: The Recent Parts](https://frontendmasters.com/courses/js-recent-parts/) [ver] [$]
- [Explorando ES2016 y ES2017](http://exploringjs.com/es2016-es2017/index.html) [leer]
- [Explorando ES2018 y ES2019](http://exploringjs.com/es2018-es2019/index.html) [leer]
- [Ilustración de expresiones regulares de JavaScript](http://codylindley.com/techpro/2013_05_14__javascript-regular-expression-/) [leer]
- [Uso de expresiones regulares](http://www.lynda.com/Regular-Expressions-tutorials/Using-Regular-Expressions/85870-2.html) [ver] [$]
- [No conoces JS: Async y rendimiento](https://github.com/getify/You-Dont-Know-JS/blob/master/async%20&%20performance/README.md#you-dont-know-js-async--performance) [leer]
- [JavaScript con promesas](http://www.amazon.com/JavaScript-Promises-Daniel-Parker/dp/1449373216/ref=pd_sim_sbs_14_5) [leer] [$]
- [Desarrollo de JavaScript basado en pruebas](http://www.amazon.com/dp/0321683919/) [leer] [$]
- [JS MythBusters](https://mythbusters.js.org/index.html) [leer]
- [Robusto JavaScript](https://molily.de/robust-javascript/) [leer]
- [Algoritmos JavaScript y estructuras de datos](https://github.com/trekhleb/javascript-algorithms#readme) [leer]
- [33 conceptos que todo desarrollador de JavaScript debe conocer](https://github.com/leonardomso/33-js-concepts) [leer]
- [doesitmutate.xyz](https://doesitmutate.xyz/) [leer]

### JavaScript funcional:

- [Jerga de programación funcional](https://github.com/hemanth/functional-programming-jargon#functional-programming-jargon)
- [funfunfunction: Programación funcional en JavaScript](https://www.youtube.com/watch?v=BMUiFMZr7vk&list=PL0zVEGEvSaeEd9hlmCXrk5yUyqUag-n84) [ver]
- [Functional-Light-JS](https://github.com/getify/Functional-Light-JS) [leer]
- [Programación funcional en JavaScript: cómo mejorar sus programas JavaScript mediante técnicas funcionales](https://www.amazon.com/Functional-Programming-JavaScript-functional-techniques/dp/1617292826/ref=sr_1_1?&_encoding=UTF8&tag=fronenddevejo-20&linkCode=ur2&linkId=dcc6b0cb7de57fa841f1b178d2d54b9d&camp=1789&creative=9325) [leer]
- [Guía principalmente adecuada para FP (en javascript)](https://drboolean.gitbooks.io/mostly-adequate-guide/content/) [leer]
- [El profesor Frisby presenta JavaScript funcional componible](https://egghead.io/courses/professor-frisby-introduces-composable-functional-javascript) [ver]
- [JavaScript Allongé](https://leanpub.com/javascriptallongesix) [leer] [$]
- [JavaScript funcional-ligero (v2)](https://frontendmasters.com/courses/functional-javascript-v2/) [ver] [$]
- [Programación funcional incondicional en JavaScript](https://frontendmasters.com/courses/functional-javascript/) [ver] [$]

### Referencias / Documentos:

- [Referencia de JavaScript de MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference)
- [Referencia de JavaScript de MSDN](https://msdn.microsoft.com/en-us/library/yek4tbz0.aspx)

### Glosario / Enciclopedia / Jerga:

- [La enciclopedia de JavaScript](http://www.crockford.com/javascript/encyclopedia/)
- [Glosario de JavaScript](https://www.codecademy.com/articles/glossary-javascript)
- [Jerga JavaScript simplificada](http://jargon.js.org/)

### Estándares / especificaciones:

- [Cómo leer la especificación ECMAScript](https://timothygu.me/es-howto/)
- [Especificación del lenguaje ECMAScript® 2015](http://www.ecma-international.org/ecma-262/6.0/index.html)
- [Especificación del lenguaje ECMAScript® 2016](https://www.ecma-international.org/ecma-262/7.0/index.html)
- [Especificación del lenguaje ECMAScript® 2017](http://www.ecma-international.org/ecma-262/8.0/index.html)
- [Especificación del lenguaje ECMAScript® 2018](http://www.ecma-international.org/ecma-262/9.0/index.html)
- [Especificación del lenguaje ECMAScript® 2019](https://tc39.github.io/ecma262/)
- [Estado, proceso y documentos para ECMA262](https://github.com/tc39/ecma262)

### Estilo:

- [Guía de estilo de JavaScript de Airbnb](http://airbnb.io/javascript/)
- [Estilo estándar de JavaScript](http://standardjs.com/rules.html)
- [Estilo semi-estándar de JavaScript](https://github.com/Flet/semistandard)

### Recursos de aprendizaje JS obsoletos:

- [Crockford en JavaScript - Volumen 1: Los primeros años](https://www.youtube.com/watch?v=JxAXlJEmNMg) [ver]
- [Crockford en JavaScript - Capítulo 2: Y luego estaba JavaScript](https://www.youtube.com/watch?v=RO1Wnu-xKoY) [ver]
- [Crockford en JavaScript - Acto III: Función máxima](https://www.youtube.com/watch?v=ya4UHuXNygM) [ver]
- [Crockford en JavaScript - Episodio IV: La metamorfosis de Ajax](https://www.youtube.com/watch?v=Fv9qT9joc0M) [ver]
- [Crockford en JavaScript - Parte 5: El fin de todas las cosas](https://www.youtube.com/watch?v=47Ceot8yqeI) [ver]
- [Crockford en JavaScript - Escena 6: Loopage](https://www.youtube.com/watch?v=QgwSUtYSUqA) [ver]
- [Patrones de JavaScript](http://www.amazon.com/gp/product/0596806752/ref=as_li_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=0596806752&linkCode=as2&tag=fronenddevejo-20&linkId=K56OPQZNQNMPF6QI) [leer] [$]
- [Los principios de JavaScript orientado a objetos](http://www.amazon.com/gp/product/1593275404/ref=as_li_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=1593275404&linkCode=as2&tag=fronenddevejo-20&linkId=NQTZVDOIMJRGMAQM) [leer] [$]
- [Módulos de JavaScript](http://jsmodules.io/cjs.html) [leer]
- [JavaScript funcional: introducción a la programación funcional con Underscore.js](http://www.amazon.com/gp/product/1449360726/ref=as_li_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=1449360726&linkCode=as2&tag=fronenddevejo-20&linkId=BDQC3FTEB3YXTYCK) [leer] [$]
- [Las partes buenas de JavaScript y la Web](https://frontendmasters.com/courses/good-parts-javascript-web/) [ver] [$]
- [JavaScript de alto rendimiento (crear interfaces de aplicaciones web más rápidas)](http://www.amazon.com/Performance-JavaScript-Faster-Application-Interfaces/dp/059680279X/ref=sr_1_1) [leer] [$]

### Exploradores / visualizadores de JS:

- [Explorador de matrices de JavaScript](https://sdras.github.io/array-explorer/)
- [Explorador de objetos JavaScript](https://sdras.github.io/object-explorer/)
- [Visualizador de JavaScript](https://tylermcginnis.com/javascript-visualizer/)

## 3.11 - Aprenda DOM, BOM, CSSOM y jQuery

> **DOM**: el modelo de objetos de documento (DOM) es una convención multiplataforma e independiente del lenguaje para representar e interactuar con objetos en documentos HTML, XHTML y XML. Los nodos de cada documento están organizados en una estructura de árbol, llamada árbol DOM. Los objetos en el árbol DOM se pueden direccionar y manipular utilizando métodos en los objetos. La interfaz pública de un DOM se especifica en su interfaz de programación de aplicaciones (API).<br>  
<div class="source">- Wikipedia</div>

> **BOM**: el modelo de objetos del navegador (BOM) es una convención específica del navegador que se refiere a todos los objetos expuestos por el navegador web. A diferencia del Modelo de objetos de documento, no existe un estándar de implementación ni una definición estricta, por lo que los proveedores de navegadores son libres de implementar la lista de materiales de la forma que deseen.<br>  
<div class="source">- Wikipedia</div>

> **jQuery**: jQuery es una biblioteca de JavaScript multiplataforma diseñada para simplificar la creación de scripts de HTML en el lado del cliente. jQuery es la biblioteca de JavaScript más popular en uso en la actualidad, con instalación en el 65% de los 10 millones de sitios con mayor tráfico en la Web. jQuery es un software gratuito de código abierto con licencia MIT.<br>  
<div class="source">- Wikipedia</div>

La ruta ideal, pero ciertamente la más difícil, sería aprender primero JavaScript, luego DOM, luego jQuery. Sin embargo, haz lo que tenga sentido para tu cerebro. La mayoría de los desarrolladores de aplicaciones para el usuario aprenden sobre JavaScript y luego sobre DOM aprendiendo primero jQuery. Cualquiera sea el camino que tome, asegúrese de que JavaScript, DOM y jQuery no se conviertan en una caja negra.

### Aprendizaje general:

- [El modelo de objetos de documento](http://eloquentjavascript.net/13_dom.html) [leer]
- [HTML/JS: hacer que las páginas web sean interactivas](https://www.khanacademy.org/computing/computer-programming/html-css-js) [ver]
- [HTML/JS: hacer que las páginas web sean interactivas con jQuery](https://www.khanacademy.org/computing/computer-programming/html-js-jquery) [ver]
- [jQuery Enlightenment](http://jqueryenlightenment.com/) [leer]
- [¿Qué es el DOM?](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction) [leer]

### Masterización:

- [Scripting DOM avanzado: Técnicas de diseño web dinámico](http://www.amazon.com/gp/product/1590598563/ref=as_li_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=1590598563&linkCode=as2&tag=fronenddevejo-20&linkId=VQZU5EQIQQXCF56Y) [leer] [$]
- [Conceptos básicos de JS avanzados para jQuery y scripts de DOM puro](https://frontendmasters.com/courses/javascript-jquery-dom/) [ver] [$]
- [Douglas Crockford: una API incómoda: la teoría del DOM](https://www.youtube.com/watch?v=Y2Y0U-2qJMs&list=PL5586336C26BDB324&index=2) [ver]
- [DOM Enlightenment](http://www.amazon.com/DOM-Enlightenment-Cody-Lindley/dp/1449342841/) [leer] [$] o [leer en línea gratis](http://domenlightenment.com/)
- [Corrección de errores comunes de jQuery](http://www.pluralsight.com/courses/fixing-common-jquery-bugs) [ver] [$]
- [JavaScript sin jQuery](http://www.pluralsight.com/courses/jquery-free-javascript) [ver] [$]
- [Consejos y trucos de jQuery](http://www.pluralsight.com/courses/jquery-tips-and-tricks) [ver] [$]

### Referencias / Documentos:

- [jQuery Docs](http://api.jquery.com/)
- [Eventos](https://html.spec.whatwg.org/#events-2)
- [Compatibilidad con el navegador DOM](http://www.webbrowsercompatibility.com/dom/desktop/)
- [Compatibilidad con el navegador de eventos DOM](http://www.webbrowsercompatibility.com/dom-events/desktop/)
- [Compatibilidad con el navegador de interfaces HTML](http://www.webbrowsercompatibility.com/html-interfaces/desktop/)
- [Modelo de objetos de documento (DOM) de MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)
- [Modelo de objetos del navegador MDN](https://developer.mozilla.org/en-US/docs/Web/API/Window)
- [Modelo de objetos de documento MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)
- [Referencia de eventos de MDN](https://developer.mozilla.org/en-US/docs/Web/Events)
- [Modelo de objetos de documento (DOM) de MSDN](https://msdn.microsoft.com/en-us/library/hh772384%28v=vs.85%29.aspx)
- [Modelo de objetos CSS (CSSOM)](https://developer.mozilla.org/en-US/docs/Web/API/CSS_Object_Model)

### Estándares / Especificaciones:

- [Modelo de objetos de documento (DOM) Nivel 3 Especificación de eventos](https://www.w3.org/TR/DOM-Level-3-Events/)
- [Informes técnicos del modelo de objetos de documento (DOM)](http://www.w3.org/DOM/DOMTR)
- [Estándar de vida DOM](https://dom.spec.whatwg.org/)
- [W3C DOM4](https://www.w3.org/TR/2015/REC-dom-20151119/)

## 3.12 - Aprenda animación web

### Aprendizaje general:

- [SVG Essentials and Animation, v2](https://frontendmasters.com/courses/svg-essentials-animation/) [$] [ver]
- [Aventuras en animaciones web](https://www.codeschool.com/courses/adventures-in-web-animations) [$] [ver]
- [Animando con Snap.svg](https://webdesign.tutsplus.com/courses/animating-with-snapsvg) [$] [ver]
- [Animación en CSS3 y HTML5](https://frontendmasters.com/courses/animation-storytelling-html5-css3/) [$] [ver]
- [Crear animaciones en CSS](http://www.kirupa.com/css_animations/index.htm) [leer y mirar]
- [Animación CSS en el mundo real](https://webdesign.tutsplus.com/courses/css-animation-in-the-real-world) [$] [ver]
- [Animación básica HTML5 con JavaScript](http://www.amazon.com/Foundation-HTML5-Animation-JavaScript-Lamberta/dp/1430236655/ref=sr_1_3) [$] [leer]
- [Aprenda a crear animaciones en JavaScript](http://www.kirupa.com/javascript_animations/index.htm) [leer y mirar]
- [Motion Design con CSS](https://frontendmasters.com/courses/motion-design-css/) [$] [ver]
- [Estado de la animación 2015](https://air.mozilla.org/rachel-nabors-state-of-the-animation-2015/) [ver]
- [Animación web con JavaScript: desarrollo y diseño](http://www.amazon.com/Web-Animation-using-JavaScript-Develop-ebook/dp/B00UNKXVDU/ref=sr_1_1) [$] [leer]

### Estándares / Especificaciones:

- [Animaciones web](https://w3c.github.io/web-animations/)

## 3.13 - Aprenda fuentes, iconos e imágenes web

> La tipografía web se refiere al uso de fuentes en la World Wide Web. Cuando se creó HTML por primera vez, las fuentes y estilos de fuente se controlaban exclusivamente mediante la configuración de cada navegador web. No había ningún mecanismo para que las páginas web individuales controlaran la visualización de fuentes hasta que Netscape introdujo la etiqueta <font> en 1995, que luego se estandarizó en la especificación HTML 3.2. Sin embargo, la fuente especificada por la etiqueta tenía que estar instalada en la computadora del usuario o se usaría una fuente alternativa, como la fuente sans-serif o monoespacio predeterminada de un navegador. La primera especificación de Hojas de estilo en cascada se publicó en 1996 y proporcionó las mismas capacidades.<br>
La especificación CSS2 se lanzó en 1998 e intentó mejorar el proceso de selección de fuentes agregando coincidencia de fuentes, síntesis y descarga. Estas técnicas no se utilizaron mucho y se eliminaron en la especificación CSS2.1. Sin embargo, Internet Explorer agregó soporte para la función de descarga de fuentes en la versión 4.0, lanzada en 1997. La descarga de fuentes se incluyó más tarde en el módulo de fuentes CSS3 y desde entonces se implementó en Safari 3.1, Opera 10 y Mozilla Firefox 3.5. Posteriormente, esto ha aumentado el interés en la tipografía web, así como en el uso de la descarga de fuentes.<br>  
<div class="source">- Wikipedia</div>

### Fuentes:

- [Una guía completa sobre las estrategias de carga de fuentes](https://www.zachleat.com/web/comprehensive-webfonts/) [leer]
- [Beautiful Web Type una muestra de los mejores tipos de letra del directorio de fuentes web de Google](http://hellohappy.org/beautiful-web-type/) [leer]
- [Guía rápida de fuentes web a través de @font-face](http://www.html5rocks.com/en/tutorials/webfonts/quick/) [leer]
- [MDN: fuentes web](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Web_fonts) [leer]
- [Tipografía web adaptable, v2](https://frontendmasters.com/courses/responsive-typography-v2/) [ver] [$]
- [Tipografía para la Web](http://www.pluralsight.com/courses/typography-for-web-1790) [ver] [$]

### Iconos:

- [leer](https://www.lynda.com/CSS-tutorials/Web-Icons-SVG/502312-2.html) [ver]

### Imágenes:

- [MDN: imágenes en HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML) [leer]
- [MDN: imágenes adaptables](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images) [leer]
- [SVG EN LA WEB - Una guía práctica](https://svgontheweb.com/) [leer]

## 3.14 - Aprenda accesibilidad

> La accesibilidad se refiere al diseño de productos, dispositivos, servicios o entornos para personas con discapacidad. El concepto de diseño accesible asegura tanto el "acceso directo" (es decir, sin asistencia) como el "acceso indirecto", lo que significa compatibilidad con la tecnología de asistencia de una persona (por ejemplo, lectores de pantalla de computadora).<br>
La accesibilidad puede verse como la "capacidad de acceder" y beneficiarse de algún sistema o entidad. El concepto se centra en permitir el acceso de personas con discapacidades o necesidades especiales, o permitir el acceso mediante el uso de tecnología de asistencia; sin embargo, la investigación y el desarrollo en accesibilidad trae beneficios para todos.<br>
La accesibilidad no debe confundirse con la usabilidad, que es la medida en que un producto (como un dispositivo, servicio o entorno) puede ser utilizado por usuarios específicos para lograr objetivos específicos con eficacia, eficiencia y satisfacción en un contexto de uso específico. La accesibilidad está fuertemente relacionada con el diseño universal, que es el proceso de creación de productos que sean utilizables por personas con la gama más amplia de habilidades posibles, que operen dentro de la gama más amplia de situaciones posibles. Se trata de hacer que las cosas sean accesibles para todas las personas (tengan o no una discapacidad).<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- [9 consejos para obtener el mínimo de accesibilidad web](https://medium.com/@realabhijeet4u/9-tips-to-get-bare-minimum-of-web-accessibility-739899a9437c)
- [Fundamentos de UX: accesibilidad](http://www.lynda.com/Accessibility-tutorials/Foundations-UX-Accessibility/435008-2.html) [ver] [$]
- [Cómo los lectores de pantalla admiten los elementos HTML](http://thepaciellogroup.github.io/AT-browser-tests/?utm_source=html5weekly&utm_medium=email) [leer]
- [Introducción a la accesibilidad web](https://www.w3.org/WAI/intro/accessibility.php) - WAI [leer]
- [Diseño universal para aplicaciones web: aplicaciones web que llegan a todos](http://www.amazon.com/Universal-Design-Web-Applications-Everyone/dp/0596518730/ref=sr_1_1) [leer] [$]
- [Accesibilidad web: introducción](http://www.pluralsight.com/courses/web-accessibility-getting-started) [ver] [$]
- [Una Web para todos](http://rosenfeldmedia.com/books/a-web-for-everyone/) [leer] [$]
- [Accesibilidad web](https://frontendmasters.com/courses/web-accessibility/) [ver] [$]
- [A11ycasts](https://www.youtube.com/playlist?list=PLNYkxOF6rcICWx0C9LVWWVqvHlYJyqw7g) [ver]
- [Accesibilidad de Google](https://www.udacity.com/course/web-accessibility--ud891): curso de Udacity [ver]

### Estándares / Especificaciones:

- [Estado actual de las aplicaciones de Internet enriquecidas accesibles](http://www.w3.org/standards/techs/aria#w3c_all) (WAI-ARIA)
- [Iniciativa de accesibilidad web (WAI)](http://www.w3.org/WAI/)
- [Estado actual de las Pautas de accesibilidad al contenido web (WCAG)](http://www.w3.org/standards/techs/wcag#w3c_all)

## 3.15 - Aprenda las API web / del navegador

![APIs de navegador](/courses/front-end-developer-handbook-2019/chapter3-7.png)

<div class="source">Fuente de la imagen: http://www.evolutionoftheweb.com/</div>

El BOM (modelo de objetos de navegador) y el DOM (modelo de objetos de documento) no son las únicas API de navegador que están disponibles en la plataforma web dentro de los navegadores. Todo lo que no es específicamente el
DOM o BOM, como una interfaz para programar el navegador podría considerarse una API web o del navegador (trágicamente en el pasado, algunas de estas API se han llamado API HTML5, lo que confunde sus propias especificaciones/estandarización con la especificación HTML5 real que especifica el lenguaje de marcado HTML5).

Tenga en cuenta que las API web o del navegador incluyen API de dispositivo (por ejemplo, ```Navigator.getBattery()```) que están disponibles a través del navegador en dispositivos de tableta y teléfono.

Debe conocer y aprender, cuando corresponda, las API de web/navegador. Una buena herramienta para familiarizarse con todas estas API sería investigar los resultados de [HTML5test.com para los 5 navegadores más actuales](https://html5test.com/compare/browser/index.html).

MDN tiene una gran cantidad de información sobre API web / navegador.

- [Referencia de la API web de MDN](https://developer.mozilla.org/en-US/docs/Web/Reference/API)
- [Referencia de la interfaz de las API web de MDN: todas las interfaces, ordenadas alfabéticamente](https://developer.mozilla.org/en-US/docs/Web/API)
- [MDN WebAPI: enumera las API de acceso a dispositivos y otras API útiles para aplicaciones](https://developer.mozilla.org/en-US/docs/WebAPI)

Tenga en cuenta que no todas las API están especificadas por el W3C o WHATWG.

Además de MDN, es posible que los siguientes recursos le resulten útiles para conocer todas las API de web/navegador:

- [El índice de la API JavaScript HTML 5](http://html5index.org/)
- [Descripción general de HTML5](http://html5-overview.net/current)
- [platform.html5.org](https://platform.html5.org/)

## 3.16 - Aprenda JSON (notación de objetos JavaScript)

> JSON, (pronunciado canónicamente a veces Notación de objetos JavaScript), es un formato estándar abierto que utiliza texto legible por humanos para transmitir objetos de datos que constan de pares atributo-valor. Es el formato de datos principal utilizado para la comunicación asincrónica entre navegador y servidor (AJAJ), y reemplaza en gran medida a XML (utilizado por AJAX).<br>
Aunque originalmente se deriva del lenguaje de secuencias de comandos de JavaScript, JSON es un formato de datos independiente del lenguaje. El código para analizar y generar datos JSON está disponible en muchos lenguajes de programación.<br>
El formato JSON fue especificado originalmente por Douglas Crockford. Actualmente está descrito por dos estándares competidores, RFC 7159 y ECMA-404. El estándar ECMA es mínimo, y describe solo la sintaxis gramatical permitida, mientras que el RFC también proporciona algunas consideraciones semánticas y de seguridad. El tipo de medio oficial de Internet para JSON es application/json. La extensión del nombre de archivo JSON es .json.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- [Introducción a la notación de objetos de JavaScript: una guía precisa para JSON](https://www.amazon.com/Introduction-JavaScript-Object-Notation-Point/dp/1491929480/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=24e8df4722cb62d086d3f8c87f4e17a1&camp=1789&creative=9325) [leer] [$]
- [json.com](https://www.json.com/) [leer]
- [¿Qué es JSON?](https://mijingo.com/lessons/what-is-json/) [ver]

### Referencias / Documentos:

- [json.org](http://json.org/) [leer]

### Estándares / Especificaciones:

- [ECMA-404 El formato de intercambio de datos JSON](http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-404.pdf)
- [RFC 7159 El formato de intercambio de datos de la notación de objetos JavaScript (JSON)](https://tools.ietf.org/html/rfc7159)
- [STD 90 - RFC 8259 - El intercambio de datos de la notación de objetos JavaScript (JSON)
Formato, DICIEMBRE 2017](https://www.rfc-editor.org/info/rfc8259)

### Arquitectura:

- [API JSON](http://jsonapi.org/)

## 3.17 - Aprenda las plantillas JS

Por lo general, se usa una plantilla de JavaScript, pero no siempre con una solución MV* para separar partes de la vista (es decir, la interfaz de usuario) de la lógica y el modelo (es decir, los datos o JSON).

- [ES6 Template Literals, ¿el asesino de los Handlebars?](https://www.keithcirkel.co.uk/es6-template-literals/) [leer]
- [Empezando con nunjucks](http://mozilla.github.io/nunjucks/getting-started.html) [leer]
[leer] [$]
- [Plantillas Lodash](https://lodash.com/docs/4.17.2#template) [docs]

Tenga en cuenta que JavaScript 2015 (también conocido como ES6) agregó un mecanismo de plantillas nativo llamado "[Cadenas de Plantillas](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/template_strings)". Además, las plantillas en los últimos tiempos han sido reemplazadas por cosas como [JSX](https://facebook.github.io/jsx/), un [elemento de plantilla](http://aurelia.io/docs/templating/basics) o [cadenas HTML](https://angular.io/docs/ts/latest/guide/template-syntax.html#).

Si no estuviera usando React & JSX, primero buscaría "[cadenas de plantillas](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/template_strings)" de JavaScript y cuando eso faltara pasar a [nunjucks](http://mozilla.github.io/nunjucks/getting-started.html).

## 3.18 - Aprenda generadores de sitios estáticos

Los generadores de sitios estáticos, generalmente escritos usando código del lado del servidor (es decir, ruby, php, python, nodeJS, etc.), producen archivos HTML estáticos a partir de texto/datos estáticos + plantillas que están destinadas a enviarse desde un servidor al cliente de forma estática sin una naturaleza dinámica.

### Aprendizaje general:

- [JAMstack](https://jamstack.org/) [leer]
- [Generadores de sitios estáticos](http://www.oreilly.com/web-platform/free/static-site-generators.csp) [leer]
- [Trabajar con sitios estáticos: llevar el poder de la simplicidad a los sitios modernos](https://www.amazon.com/Working-Static-Sites-Bringing-Simplicity/dp/1491960949) [leer] [$]

## 3.19 - Aprenda informática a través de JS

- [Cuatro semestres de informática en seis horas](https://frontendmasters.com/courses/computer-science/) [video] [$]
- [Cuatro semestres de informática en seis horas: Parte 2](https://frontendmasters.com/courses/computer-science-2/) [video] [$]
- [Ciencias de la computación en JavaScript](https://github.com/davidshariff/computer-science) [leer]
- [Colección de paradigmas, algoritmos y enfoques clásicos de la informática escritos en JavaScript](https://github.com/nzakas/computer-science-in-javascript) [leer]
- [Una guía práctica de algoritmos con JavaScript](https://frontendmasters.com/courses/practical-algorithms/) [ver] [$]
- [Introducción a las estructuras de datos para entrevistas](https://frontendmasters.com/courses/data-structures-interviews/) [ver] [$]
- [Clase magistral de estructuras de datos y algoritmos JavaScript](https://www.udemy.com/js-algorithms-and-data-structures-masterclass/) [ver] [$]

## 3.20 - Aprenda la arquitectura de aplicaciones front-end

### Aprendizaje general:

- [Guía front-end de Grab](https://github.com/grab/front-end-guide) [leer]
- [Un conjunto de mejores prácticas para proyectos de JavaScript](https://github.com/elsewhencode/project-guidelines)
- [Libro de hechizos del desarrollador web moderno](https://github.com/dexteryy/spellbook-of-modern-webdev)
- [Pila de JavaScript desde cero](https://github.com/verekia/js-stack-from-scratch)

### Materiales de aprendizaje obsoletos:

- [Diseño de aplicaciones JavaScript](https://www.amazon.com/JavaScript-Application-Design-Build-Approach/dp/1617291951?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=4dd15b53493d3b5148af2b3e5488e98d&camp=1789&creative=9325) [leer] [$]
- [Cree una aplicación con React y Ampersand](http://learn.humanjavascript.com/react-ampersand) [ver]
- [Guía de campo para aplicaciones web](http://www.html5rocks.com/webappfieldguide/toc/index/) [leer]
- [Cuestionario de directrices de frontend](https://github.com/bradfrost/frontend-guidelines-questionnaire) [leer]
- [JavaScript humano](http://read.humanjavascript.com/) [leer]
- [Nicholas Zakas: Arquitectura de aplicaciones JavaScript escalable](https://www.youtube.com/watch?v=vXjVFPosQHw) [ver]
- [Organizar la funcionalidad de JavaScript](https://frontendmasters.com/courses/organizing-javascript/) [ver] [$]
- [Patrones para la arquitectura de aplicaciones JavaScript a gran escala](http://addyosmani.com/largescalejavascript/) [leer]
- [Terrific](http://terrifically.org/) [leer]
- [Estudios de caso de frontend](https://github.com/andrew--r/frontend-case-studies) [leer]

Últimamente no se está creando mucho contenido general sobre este tema. La mayor parte del contenido que se ofrece para aprender a crear aplicaciones front-end/SPA/JavaScript presupone que ha elegido una herramienta como Angular, Ember, React o Aurelia.

Mi consejo, en [2019](https://2018.stateofjs.com/front-end-frameworks/overview/) aprenda [React](https://facebook.github.io/react/) y [Mobx](https://github.com/mobxjs/mobx) y [Apollo/graphql](https://www.apollographql.com/).

## 3.21 - Aprenda Data (es decir, JSON) API Design

- [Diseño de API, v3](https://frontendmasters.com/courses/api-design-nodejs-v3/) [ver] [$]
- [Cree API que no odiará](http://apisyouwonthate.com/) [$] [leer]
- [API JSON](http://jsonapi.org/) [leer]

## 3.22 - Aprenda React

### Aprendiendo React:

- [Tutorial: Introducción a reaccionar](https://facebook.github.io/react/tutorial/tutorial.html) [leer]
- [ReactJS para gente estúpida](http://blog.andrewray.me/reactjs-for-stupid-people/) [leer]
- [La guía para principiantes de ReactJS](https://egghead.io/courses/the-beginner-s-guide-to-reactjs) [ver]
- [Introducción completa a React v4](https://frontendmasters.com/courses/complete-react-v4/) [ver] [$]
- [React](https://react.holiday/) [leer]
- [Suscripción de video de React Patterns](https://school.reactpatterns.com/) [ver] [$]
- [React Enlightenment](https://www.reactenlightenment.com/) [leer]
- [TUTORIAL DE REACT JS # 1 - Introducción a Reactjs Javascript y configuración del espacio de trabajo](https://www.youtube.com/watch?v=MhkGQAoc7bc&t=6s) [ver]

### Dominando React:

- [Cree su primera aplicación React de calidad de producción](https://egghead.io/courses/build-your-first-production-quality-react-app) [ver] [$]
- [Patrones avanzados de componentes de React](https://frontendmasters.com/courses/advanced-react-patterns/) [ver] [$]
- [React intermedio](https://frontendmasters.com/courses/intermediate-react/) [ver] [$]
- [Patrones React](https://reactpatterns.com/) [leer]
- [8 decisiones clave del componente React](https://medium.freecodecamp.org/8-key-react-component-decisions-cc965db11594) [leer]
- [React - Conceptos teóricos básicos](https://github.com/reactjs/react-basic) [leer]
- [Base de código de React + Mobx que contiene ejemplos del mundo real (CRUD, autenticación, patrones avanzados, etc.) que se adhieren a las especificaciones y API de RealWorld.](https://github.com/gothinkster/react-mobx-realworld-example-app) [código]
- [Introducción a React Router v4 y su filosofía hacia el enrutamiento](https://medium.freecodecamp.org/react-router-v4-philosophy-and-introduction-730fd4fff9bc) [leer]

Una vez que tenga un buen manejo de React, continúe con el aprendizaje de una solución de administración de estado más sólida como [MobX](https://mobx.js.org/). Si eres un desarrollador experimentado con conocimientos de programación funcional, mira [Redux](https://redux.js.org/). Si necesita ayuda para comprender el papel de la administración de estado más allá de ver ```setState``` de React, "[Administración de estado avanzada en React (con Redux y MobX)](https://frontendmasters.com/courses/react-state/)".

## 3.23 - Aprenda la gestión del estado de la aplicación

- [Gestión de estado en JavaScript](https://codeburst.io/state-management-in-javascript-15d0d98837e1) [leer]
- [Gestión avanzada del estado en React (con Redux y MobX)](https://frontendmasters.com/courses/react-state/) [ver] [$]
- [Tutorial de React js - Cómo funciona Redux](https://www.youtube.com/watch?v=1w-oQ-i1XB8&list=PLoYCgNOIyGADILc3iUJzygCqC8Tt3bRXt) [ver]
- [MobX + React es IMPRESIONANTE](https://www.youtube.com/watch?v=_q50BXqkAfI&t=10s) [ver]

## 3.24 - Aprenda la aplicación web progresiva

> A diferencia de las aplicaciones tradicionales, las aplicaciones web progresivas son un híbrido de páginas web (o sitios web) normales y una aplicación móvil. Este nuevo modelo de aplicación intenta combinar las características que ofrecen la mayoría de los navegadores modernos con los beneficios de la experiencia móvil.<br>
En 2015, la diseñadora Frances Berriman y el ingeniero de Google Chrome Alex Russell acuñaron el término "Aplicaciones web progresivas" para describir las aplicaciones que aprovechan las nuevas funciones compatibles con los navegadores modernos, incluidos Service Workers y Manifiestos de aplicaciones web, que permiten a los usuarios actualizar las aplicaciones web para ser aplicaciones de primera clase en su sistema operativo nativo.<br>
Según Google Developers, estas características son:<br>
> - Progresivo: funciona para todos los usuarios, independientemente de la elección del navegador, ya que se construyeron con la mejora progresiva como principio fundamental.
> - Capacidad de respuesta: se adapta a cualquier factor de forma: escritorio, dispositivo móvil, tableta o formularios que aún no han aparecido.
> - Independiente de la conectividad: los trabajadores del servicio permiten trabajar sin conexión o en redes de baja calidad.
> - Similar a una aplicación: siéntase como una aplicación para el usuario con interacciones y navegación al estilo de una aplicación.
> - Fresco: siempre actualizado gracias al proceso de actualización del trabajador de servicio.
> - Seguro: se sirve a través de HTTPS para evitar espionaje y garantizar que el contenido no haya sido manipulado.
> - Descubribles: se pueden identificar como "aplicaciones" gracias a los manifiestos del W3C [6] y al alcance de registro del trabajador de servicios que permite a los motores de búsqueda encontrarlas.
> - Re-interacción: facilite la re-interacción a través de funciones como notificaciones automáticas.
> - Instalable: permite a los usuarios "conservar" las aplicaciones que encuentran más útiles en su pantalla de inicio sin la molestia de una tienda de aplicaciones.
> - Vinculable: se comparte fácilmente a través de una URL y no requiere una instalación compleja.<br>  
<div class="source">- Wikipedia</div>

- [Una guía para principiantes sobre aplicaciones web progresivas](https://www.smashingmagazine.com/2016/08/a-beginners-guide-to-progressive-web-apps/) [leer]
- [Aplicaciones web progresivas](https://developers.google.com/web/progressive-web-apps/) [leer]
- [Introducción a las aplicaciones web progresivas](https://www.pluralsight.com/courses/web-apps-progressive-getting-started) [ver] [$]
- [Creación de una aplicación web progresiva](https://www.lynda.com/CSS-tutorials/Building-Progressive-Web-App/518052-2.html) [ver] [$]
- [Introducción a las aplicaciones web progresivas de Google](https://www.udacity.com/course/intro-to-progressive-web-apps--ud811) [ver]
- [Las aplicaciones nativas están condenadas](https://medium.com/javascript-scene/native-apps-are-doomed-ac397148a2c0#.rfw9hdym6) [leer]
- [Por qué las aplicaciones nativas están realmente condenadas: las aplicaciones nativas están condenadas pt 2](https://medium.com/javascript-scene/why-native-apps-really-are-doomed-native-apps-are-doomed-pt-2-e035b43170e9#.qjrm13yj3) [leer]
- [Tu primera aplicación web progresiva](https://developers.google.com/web/fundamentals/codelabs/your-first-pwapp/) [leer]
- [Aplicaciones web progresivas y sin conexión](https://frontendmasters.com/courses/progressive-web-apps/) [ver] [$]

## 3.25 - Aprenda el diseño de API JS

- [Diseñar mejores API de JavaScript](http://www.smashingmagazine.com/2012/10/designing-javascript-apis-usability/) [leer]
- [Escribir API de JavaScript](http://blog.wolksoftware.com/writing-javascript-apis) [leer]

## 3.26 - Aprenda las herramientas de desarrollo web del navegador

> Las herramientas de desarrollo web permiten a los desarrolladores web probar y depurar su código. Se diferencian de los creadores de sitios web y los IDE en que no ayudan en la creación directa de una página web, sino que son herramientas que se utilizan para probar la interfaz de usuario de un sitio web o aplicación web.<br>
Las herramientas de desarrollo web vienen como complementos del navegador o funciones integradas en los navegadores web. Los navegadores web más populares de la actualidad, como Google Chrome, Firefox, Opera, Internet Explorer y Safari, tienen herramientas integradas para ayudar a los desarrolladores web, y se pueden encontrar muchos complementos adicionales en sus respectivos centros de descarga de complementos.<br>
Las herramientas de desarrollo web permiten a los desarrolladores trabajar con una variedad de tecnologías web, incluidos HTML, CSS, DOM, JavaScript y otros componentes que maneja el navegador web. Debido a la creciente demanda de los navegadores web para hacer, los navegadores web más populares han incluido más funciones orientadas a los desarrolladores.<br>  
<div class="source">- Wikipedia</div>

Si bien la mayoría de los navegadores vienen equipados con herramientas de desarrollo web, las [herramientas de desarrollo de Chrome](https://developers.google.com/web/tools/chrome-devtools/) son actualmente las más comentadas y utilizadas.

Sugeriría aprender y usar las herramientas de desarrollo web de Chrome, simplemente porque los mejores recursos para aprender herramientas de desarrollo web giran en torno a Chrome DevTools.

### Aprenda las herramientas para desarrolladores web de Chrome:

- [Herramientas para desarrolladores de Chrome](https://code.tutsplus.com/courses/chrome-developer-tools) [ver] [$]
- [Explore y domine las DevTools de Chrome](http://discover-devtools.codeschool.com/) [ver]
- [Dominar las herramientas para desarrolladores de Chrome v2](https://frontendmasters.com/courses/chrome-dev-tools-v2/) [ver] [$]
- [Uso de las herramientas para desarrolladores de Chrome](http://www.pluralsight.com/courses/chrome-developer-tools) [ver] [$]
- [Aprenda las herramientas para desarrolladores web de Chrome](https://www.lynda.com/Chrome-tutorials/Learning-Chrome-Web-Developer-Tools/590844-2.html) [ver] [$]

### Documentos de herramientas para desarrolladores web de Chrome:

- [Referencia de la API de línea de comandos](https://developers.google.com/web/tools/chrome-devtools/console/command-line-reference)
- [Referencia de atajos de teclado e interfaz de usuario](https://developers.google.com/web/tools/iterate/inspect-styles/shortcuts)
- [Documentación por panel](https://developers.google.com/web/tools/chrome-devtools/#docs)
- [Configurar y personalizar DevTools](https://developer.chrome.com/devtools/docs/settings)

## 3.27 - Aprenda la línea de comandos (también conocida como CLI)

> Una interfaz de línea de comandos o un intérprete de lenguaje de comandos (CLI), también conocida como interfaz de usuario de línea de comandos, interfaz de usuario de consola e interfaz de usuario de caracteres (CUI), es un medio de interactuar con un programa de computadora cuando el usuario (o cliente) tiene problemas comandos al programa en forma de líneas sucesivas de texto (líneas de comando).<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- [La guía de Bash](http://guide.bash.academy/) [leer]
- [Usuario avanzado de la línea de comandos](http://commandlinepoweruser.com/) [ver]
- [Aprenda suficiente línea de comandos para ser peligroso](http://www.learnenough.com/command-line-tutorial) [leer] [de gratis a $]

### Masterización:

- [Técnicas avanzadas de línea de comandos](https://code.tutsplus.com/courses/advanced-command-line-techniques) [ver] [$]
- [Introducción a Bash, VIM y Regex](https://frontendmasters.com/courses/bash-vim-regex/) [ver] [$]

## 3.28 - Aprenda Node.js

> Node.js es un entorno de ejecución multiplataforma de código abierto para desarrollar aplicaciones web del lado del servidor. Las aplicaciones de Node.js están escritas en JavaScript y se pueden ejecutar dentro del tiempo de ejecución de Node.js en OS X, Microsoft Windows, Linux, FreeBSD, NonStop, IBM AIX, IBM System z e IBM i. Su trabajo está alojado y respaldado por Node.js Foundation, un proyecto colaborativo en Linux Foundation.<br> Node.js proporciona una arquitectura impulsada por eventos y una API de E/S sin bloqueo diseñada para optimizar el rendimiento y la escalabilidad de una aplicación en tiempo real. Utiliza el motor JavaScript Google V8 para ejecutar código y un gran porcentaje de los módulos básicos están escritos en JavaScript. Node.js contiene una biblioteca incorporada para permitir que las aplicaciones actúen como un servidor web sin software como Apache HTTP Server, Nginx o IIS.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- [El arte de Node](https://github.com/maxogden/art-of-node#the-art-of-node) [leer]
- [Introducción a Node.js](https://frontendmasters.com/courses/node-js/) [ver] [$]
- [Introducción a Node.js de Evented Mind](https://www.eventedmind.com/classes/introduction-to-node-js-4c0326de) [ver]
- [io.js y Node.js Siguiente: Primeros pasos](http://www.pluralsight.com/courses/running-node-applications-io-js) [ver] [$]
- [Aprendiendo Node: Pasar al lado del servidor](https://www.amazon.com/Learning-Node-Server-Side-Shelley-Powers/dp/1491943122/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=264ce29eb0775f4e8ccb7db892539555&camp=1789&creative=9325) [leer] [$]
- [Learn You The Node.js](https://github.com/workshopper/learnyounode) [talleres autoguiados]
- [Conceptos básicos de Node.js](http://teamtreehouse.com/library/nodejs-basics) [ver] [$]
- [Node.js en la práctica](https://www.amazon.com/Node-js-Practice-Alex-R-Young/dp/1617290939/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=e202c01e97ebad79157fab3b59723e94&camp=1789&creative=9325) [leer] [$]
- [Web en tiempo real con Node.js](https://www.codeschool.com/courses/real-time-web-with-node-js) [ver]
- [Diseño de API en Node.js, v3](https://frontendmasters.com/courses/api-design-nodejs-v3/) [ver] [$]
- [Aprenda Node](https://learnnode.com/) [ver] [$]

## 3.29 - Aprenda módulos

### Aprendizaje general:

- [JavaScript para programadores impacientes - Módulos](http://exploringjs.com/impatient-js/ch_modules.html) [leer]
- [Módulos ES6 en profundidad](https://ponyfoo.com/articles/es6-modules-in-depth) [leer]
- [Explorando JS - Módulos](http://exploringjs.com/es6/ch_modules.html#ch_modules) [leer]
- [Módulos ES: un análisis profundo de dibujos animados](https://hacks.mozilla.org/2018/03/es-modules-a-cartoon-deep-dive/) [leer]

### Referencias / Documentos:

- [MDN - exportación](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/export)
- [MDN - importación](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import)

## 3.30 - Aprenda módulos cargadores/agrupadores

### Webpack:

- [Webpack](https://webpack.js.org/guides/getting-started/) [leer]
- [Conceptos básicos de Webpack 4](https://frontendmasters.com/courses/webpack-fundamentals/) [ver] [$]
- [Libro de paquete web de Survivejs.com](https://survivejs.com/webpack/introduction/) [leer]

### Rollup:

- [Rollup](http://rollupjs.org/guide/) [leer]
  - [Microbundle](https://github.com/developit/microbundle)

### Parcel

- [Parcel](https://parceljs.org/getting_started.html) [leer]

## 3.31 - Aprenda administrador de paquetes

> Un administrador de paquetes o sistema de administración de paquetes es una colección de herramientas de software que automatiza el proceso de instalación, actualización, configuración y eliminación de paquetes de software para el sistema operativo de una computadora de manera consistente. Por lo general, mantiene una base de datos de dependencias de software e información de versión para evitar discrepancias de software y requisitos previos faltantes.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- [Introducción a cómo funcionan los administradores de paquetes de JavaScript](https://medium.freecodecamp.com/javascript-package-managers-101-9afd926add0a#.hu6knvct3) [leer]
- [Los rangos de SemVer místicos y mágicos utilizados por npm & Bower](http://developer.telerik.com/featured/mystical-magical-semver-ranges-used-npm-bower/) [leer]
- [Administradores de paquetes: una guía introductoria para el desarrollador front-end no iniciado](http://codylindley.com/techpro/2013_04_12__package-managers-an-introducto/) [leer]
- [Documentos sobre npm](https://docs.npmjs.com/)
- [Documentos sobre yarn](https://yarnpkg.com/en/docs/)

## 3.32 - Aprenda control de versiones

> Un componente de la gestión de la configuración del software, el control de versiones, también conocido como control de revisión o control de fuente, es la gestión de cambios en documentos, programas informáticos, sitios web grandes y otras colecciones de información. Los cambios generalmente se identifican mediante un código numérico o de letras, denominado "número de revisión", "nivel de revisión" o simplemente "revisión". Por ejemplo, un conjunto inicial de archivos es "revisión 1". Cuando se realiza el primer cambio, el conjunto resultante es "revisión 2" y así sucesivamente. Cada revisión está asociada con una marca de tiempo y la persona que realiza el cambio. Las revisiones se pueden comparar, restaurar y combinar con algunos tipos de archivos.<br>  
<div class="source">- Wikipedia</div>

La solución más común utilizada hoy para el [control de versiones](https://en.wikipedia.org/wiki/Version_control) es [Git](https://git-scm.com/). ¡Apréndalo!

### Aprendizaje general:

- [Haciendo lo correcto](https://www.atlassian.com/git/) [leer]
- [Conceptos básicos de Git](http://www.pluralsight.com/courses/git-fundamentals) [ver] [$]
- [Aprenda lo suficiente de Git](https://www.learnenough.com/git-tutorial) [leer]
- [Tutorial Git de Ry](https://www.amazon.com/Rys-Git-Tutorial-Ryan-Hodson-ebook/dp/B00QFIA5OC) [leer]

### Masterización:

- [Git en profundidad](https://frontendmasters.com/courses/git-in-depth/) [ver] [$]
- [Tutoriales avanzados de Git](https://www.atlassian.com/git/tutorials/advanced-overview/) [leer]
- [Pro Git](http://git-scm.com/book/en/v2) [leer]
- [Más información sobre la ramificación de Git](http://learngitbranching.js.org/) [interactuar]

### Referencias / Documentos:

- https://git-scm.com/doc
- [git-cheatsheet](https://gist.github.com/eashish93/3eca6a90fef1ea6e586b7ec211ff72a5)

## 3.33 - Aprenda la automatización de tareas y compilaciones

> La automatización de compilaciones es el proceso de automatizar la creación de una compilación de software y los procesos asociados que incluyen: compilar el código fuente de la computadora en código binario, empaquetar código binario y ejecutar pruebas automatizadas.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- [Introducción a Gulp](https://www.amazon.com/Getting-Started-Gulp-Travis-Maynard/dp/1784395765?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=3eb1e7a868a09b44f90570c56ef5f53b&camp=1789&creative=9325) [leer] [$]
- [Conceptos básicos de Gulp](http://teamtreehouse.com/library/gulp-basics) [ver] [$]
- [Automatización de compilación de JavaScript con Gulp.js](http://www.pluralsight.com/courses/javascript-build-automation-gulpjs) [ver] [$]

### Referencias / Documentos:

- [Gulp](https://github.com/gulpjs/gulp/blob/master/docs/getting-started.md)

Gulp es genial. Sin embargo, es posible que solo necesite ```npm run```. Antes de pasar a la complejidad adicional en su pila de aplicaciones, pregúntese si ```npm run``` puede hacer el trabajo. Si necesitas más, usa Gulp.

Lee:

- [¡Dale la Boot a Grunt! Una guía para usar npm como herramienta de compilación](http://www.sitepoint.com/guide-to-npm-as-a-build-tool/)
- [Usando npm como un sistema de compilación para su próximo proyecto](https://drublic.de/blog/npm-builds)
- [Uso de npm como Task Runner](http://teamtreehouse.com/library/using-npm-as-a-task-runner) [ver] [$]
- [Por qué dejé Gulp y Grunt por scripts npm?](https://medium.freecodecamp.com/why-i-left-gulp-and-grunt-for-npm-scripts-3d6853dd22b8#.z8plsoxxs)
- [Por qué npm Scripts?](https://css-tricks.com/why-npm-scripts/)

## 3.34 - Aprenda sobre la optimización del rendimiento del sitio

> La optimización del rendimiento web, WPO u optimización del sitio web es el campo de conocimiento sobre cómo aumentar la velocidad en la que las páginas web se descargan y se muestran en el navegador web del usuario. Dado que la velocidad promedio de Internet aumenta a nivel mundial, es apropiado que los administradores de sitios web y los webmasters consideren el tiempo que tardan los sitios web en mostrarse para el visitante.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- [Optimización de la representación del navegador](https://www.udacity.com/course/browser-rendering-optimization--ud860) [ver]
- [Sitios web aún más rápidos: mejores prácticas de rendimiento para desarrolladores web](https://www.amazon.com/Even-Faster-Web-Sites-Performance/dp/0596522304?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=4fe6a82bbf727209ba337ecaa0e516bc&camp=1789&creative=9325) [leer] [$]
- [Sitios web de alto rendimiento: conocimientos esenciales para los ingenieros de front-end](https://www.amazon.com/High-Performance-Web-Sites-Essential/dp/0596529309/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=e93ab3ea06b7e3e93ee0d868249d0e3f&camp=1789&creative=9325) [leer] [$]
- [El rendimiento de JavaScript Rocks](http://javascriptrocks.com/) [leer] [$]
- [Reglas de PageSpeed ​​Insights](https://developers.google.com/speed/docs/insights/rules) [leer]
- [perf-tooling.today](http://www.perf-tooling.today/) [leer]
- [Calendario de rendimiento](http://calendar.perfplanet.com/) [leer]
- [perf.rocks](http://perf.rocks/) [leer]
- [Usando WebPageTest](https://www.amazon.com/Using-WebPageTest-Rick-Viscomi/dp/1491902590/ref=sr_1_1?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=91a76d5d4b4f47cf4e0d1392cc9cea30&camp=1789&creative=9325) [leer] [$]
- [Libro diario de rendimiento web, volumen 2](https://www.amazon.com/Web-Performance-Daybook-Techniques-Optimizing/dp/1449332919/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=59e32c394c2377bb17af1d801b924d1d&camp=1789&creative=9325) [leer] [$]
- [Rendimiento del sitio web](https://frontendmasters.com/courses/web-performance/) [ver] [$]
- [Rendimiento web con Webpack 4](https://frontendmasters.com/courses/performance-webpack/) [ver] [$]
- [Optimización del rendimiento del sitio web](https://www.udacity.com/course/website-performance-optimization--ud884) [ver]
- [Lista de verificación de rendimiento de front-end 2019 (PDF, páginas de Apple, MS Word)](https://www.smashingmagazine.com/2019/01/front-end-performance-checklist-2019-pdf-pages/) [leer]

## 3.35 - Aprenda a realizar pruebas

> **Pruebas unitarias**: en programación de computadoras, las pruebas unitarias son un método de prueba de software mediante el cual unidades individuales de código fuente, conjuntos de uno o más módulos de programas de computadora junto con el control asociado
Los datos, los procedimientos de uso y los procedimientos operativos se prueban para determinar si son aptos para su uso. Intuitivamente, uno puede ver una unidad como la parte más pequeña que se puede probar de una aplicación.<br>  
<div class="source">- Wikipedia</div>

> **Pruebas funcionales**: las pruebas funcionales son un proceso de garantía de calidad (QA) y un tipo de prueba de caja negra que basa sus casos de prueba en las especificaciones del componente de software bajo prueba. Las funciones se prueban alimentándolas de entrada y examinando la salida, y la estructura interna del programa rara vez se considera (no como en las pruebas de caja blanca). Las pruebas funcionales generalmente describen lo que hace el sistema.<br>  
<div class="source">- Wikipedia</div>

> **Pruebas de integración**: las pruebas de integración (a veces llamadas integración y pruebas, abreviado I&T) es la fase de las pruebas de software en la que los módulos de software individuales se combinan y prueban como un grupo. Ocurre después de las pruebas unitarias y antes de las pruebas de validación. La prueba de integración toma como entrada los módulos que han sido probados por unidad, los agrupa en agregados más grandes, aplica las pruebas definidas en un plan de prueba de integración a esos agregados y entrega como salida el sistema integrado listo para la prueba del sistema.<br>  
<div class="source">- Wikipedia</div>

### Aprendizaje general:

- [Principios y prácticas de prueba de JavaScript](https://frontendmasters.com/courses/testing-practices-principles/) [ver] [$]
- [Primero, el front-end: prueba y creación de prototipos de aplicaciones JavaScript](http://www.pluralsight.com/courses/testing-and-prototyping-javascript-apps) [ver] [$]
- [Let's Code: JavaScript basado en pruebas](http://www.letscodejavascript.com/) [ver] [$]
- [Prueba de JavaScript](https://www.udacity.com/course/javascript-testing--ud549) [ver]
- [Recetas de prueba de JavaScript](http://jstesting.jcoglan.com/) [leer] [$]
- [JavaScript comprobable](https://www.amazon.com/gp/product/1449323391?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=a27df21b09e3eff9ad8033a5c959e7f0&camp=1789&creative=9325) [leer] [$]
- [Pruebas de aplicaciones de JavaScript: código rápido, seguro y que se puede mantener](https://www.amazon.com/Test-Driving-JavaScript-Applications-Confident-Maintainable/dp/1680501747?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=c97c9c87e634569328a335cba0b0c15f&camp=1789&creative=9325) [leer] [$]
- [Desarrollo de JavaScript basado en pruebas](https://www.amazon.com/dp/0321683919/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=f707aa5243bf6bac68bda05d1e6369e8&camp=1789&creative=9325) [leer] [$]
- [The Way of the Web Tester: Guía para principiantes sobre la automatización de pruebas](https://www.amazon.com/Way-Web-Tester-Beginners-Automating/dp/1680501836/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=3e2c87950e0350d64c9d9862ed2ef524&camp=1789&creative=9325) [leer] [$]
- [Prueba de aplicaciones React, v2](https://frontendmasters.com/courses/testing-react/) [ver] [$]
- [Aprenda las pruebas unitarias de JavaScript con Mocha, Chai y Sinon](https://www.udemy.com/learn-javascript-unit-testing-with-mocha-chai-and-sinon/) [ver] [$]

## 3.36 - Aprenda los navegadores sin cabeza

> Un navegador sin cabeza es un navegador web sin una interfaz gráfica de usuario.<br>
Los navegadores sin cabeza proporcionan control automatizado de una página web en un entorno similar a los navegadores web populares, pero se ejecutan a través de una interfaz de línea de comandos o mediante la comunicación de red. Son particularmente útiles para probar páginas web, ya que pueden representar y comprender HTML de la misma manera que lo haría un navegador, incluidos elementos de estilo como diseño de página, color, selección de fuentes y ejecución de JavaScript y AJAX que generalmente no están disponibles cuando se usa otros métodos de prueba. Google declaró en 2009 que el uso de un navegador sin cabeza podría ayudar a su motor de búsqueda a indexar el contenido de los sitios web que usan AJAX.<br>  
<div class="source">- Wikipedia</div>

- [Introducción a Headless Chrome](https://developers.google.com/web/updates/2017/04/headless-chrome) [léame]

[PhantomJS ya no se mantiene](https://www.infoq.com/news/2017/04/Phantomjs-future-uncertain), [Headless Chrome](https://chromium.googlesource.com/chromium/src/+/lkgr/headless/README.md) interviene.

## 3.37 - Aprenda desarrollo sin conexión

El desarrollo fuera de línea (también conocido como fuera de línea primero) es un área de conocimiento y discusión en torno a las prácticas de desarrollo para dispositivos que no siempre están conectados a Internet o a una fuente de alimentación.

### Aprendizaje general:

- [Creación de aplicaciones web HTML5 sin conexión](http://apress.jensimmons.com/v5/pro-html5-programming/ch12.html) [leer]
- [Todo lo que necesita saber para crear aplicaciones web sin conexión primero](https://github.com/pazguille/offline-first) [leer]
- [Sin conexión primero](http://www.webdirections.org/offlineworkshop/ibooksDraft.pdf) [leer]
- [offlinefirst.org](http://offlinefirst.org/) [leer]
- [El libro de cocina sin conexión](https://developers.google.com/web/fundamentals/instant-and-offline/offline-cookbook/) [leer]
- [Inicio rápido sin conexión](https://developers.google.com/web/ilt/pwa/offline-quickstart) [leer]

## 3.38 - Aprenda seguridad web/navegador/app

- [Manual de seguridad del navegador](https://code.google.com/p/browsersec/wiki/Main) [leer]
- [Seguridad frontend](https://mikewest.org/2013/09/frontend-security-frontendconf-2013) [ver]
- [Hacksplaining](https://www.hacksplaining.com/) [leer]
- [Hoja de referencia de seguridad HTML5](https://html5sec.org/) [leer]
- [Prácticas recomendadas de seguridad HTTP](https://httpsecurityreport.com/best_practice.html) [leer]
- [Seguridad de identidad y datos para el desarrollo web: prácticas recomendadas](https://www.amazon.com/Identity-Data-Security-Web-Development/dp/1491937017?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=f5f2aaa4d5f944a3ccc316a16e3673f4&camp=1789&creative=9325) [leer](https://frontendmasters.com/books/front-end-handbook/2019/$)
- [Seguridad para desarrolladores web: uso de JavaScript, HTML y CSS](https://www.amazon.com/Security-Web-Developers-Using-JavaScript/dp/1491928646/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=df49be399d7d1a12acebe5a85637a7a8&camp=1789&creative=9325) [leer] [$]
- [Conceptos básicos de la seguridad de las aplicaciones web](http://martinfowler.com/articles/web-security-basics.html) [leer]
- [Internet: cifrado y claves públicas](https://www.youtube.com/watch?v=ZghMPWGXexs&list=PLzdnOPI1iJNfMRZm5DDxco3UdsFegvuB7&index=6) [ver]
- [Internet: ciberseguridad y delitos](https://www.youtube.com/watch?v=AuYNXgO_f3Y&list=PLzdnOPI1iJNfMRZm5DDxco3UdsFegvuB7&index=7) [ver]
- [The Tangled Web: Una guía para proteger las aplicaciones web modernas](http://lcamtuf.coredump.cx/tangled/) [leer] [$]
- [Conceptos básicos de seguridad web](https://github.com/vasanthk/web-security-basics) [leer]
- [Seguridad web](https://developer.mozilla.org/en-US/docs/Web/Security) [leer]
- [Seguridad web](https://frontendmasters.com/courses/web-security/) [ver] [$]
- [Pila completa para ingenieros de front-end](https://frontendmasters.com/courses/full-stack/) [ver] [$]

## 3.39 - Aprenda el desarrollo multidispositivo

![Esto será la web](/courses/front-end-developer-handbook-2019/chapter3-8.png)

<div class="source">Fuente de la imagen: http://bradfrost.com/blog/post/this-is-the-web/</div>

Un sitio web o una aplicación web puede ejecutarse en una amplia gama de computadoras, portátiles, tabletas y teléfonos, así como en un puñado de dispositivos nuevos (relojes, termostatos, refrigeradores, etc.). La forma en que determina qué dispositivos admitirá y cómo desarrollará para admitir esos dispositivos se denomina "estrategia de desarrollo de dispositivos múltiples". A continuación, enumero las estrategias de desarrollo multidispositivo más comunes.

- Cree un sitio web/aplicación [responsive (RWD)](https://en.wikipedia.org/wiki/Responsive_web_design) para todos los dispositivos.
- Cree un sitio web/aplicación [adaptable/progresivamente](https://en.wikipedia.org/wiki/Adaptive_web_design) mejorado para todos los dispositivos.
- Cree un sitio web, una aplicación web, una aplicación nativa o una aplicación nativa híbrida para cada dispositivo individual o grupo de dispositivos.
- Intente modernizar algo que ya ha construido utilizando bits y partes de las estrategias 1, 2 o 3.

### Aprendizaje general:

- [Un libro Apart Pack - Diseño web adaptable](https://abookapart.com/collections/responsive-design) [leer] [$]
- [Un paquete de libro aparte: diseño para cualquier dispositivo](https://abookapart.com/collections/design-for-any-device) [leer] [$]
- [Diseño web adaptable](https://www.amazon.com/gp/product/0134216148?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=defa398e66db76e7edbb8ddfa28caa1e&camp=1789&creative=9325) [leer] [$]
- [Diseñar con mejora progresiva](https://www.amazon.com/Designing-Progressive-Enhancement-Building-Everyone/dp/0321658884/?&_encoding=UTF8&tag=frontend-handbook-20&linkCode=ur2&linkId=bdac6f12a3d24fe694468aa8145001eb&camp=1789&creative=9325) [leer] [$]
- [Desarrollo web móvil](https://www.udacity.com/course/mobile-web-development--cs256) [ver]
- [CSS Grids y Flexbox para diseño web adaptable](https://frontendmasters.com/courses/css-grids-flexbox/) [ver] [$]
- [Diseño de email HTML receptivo](https://frontendmasters.com/courses/responsive-email/) [ver] [$]
- [Imágenes receptivas](https://www.udacity.com/course/responsive-images--ud882) [ver]
- [Tipografía web adaptable, v2](https://frontendmasters.com/courses/responsive-typography-v2/) [ver] [$]
- [Conceptos básicos del diseño web adaptable](https://www.udacity.com/course/responsive-web-design-fundamentals--ud893) [ver]
