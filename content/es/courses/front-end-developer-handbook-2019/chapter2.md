---
title: Capítulo 2. La práctica del desarrollo front-end. Descripción general
linktitle: Capítulo2. La práctica del desarrollo front-end. Descripción general
toc: true
type: docs
date: "2020-09-03T00:00:00+01:00"
draft: false
menu:
  front-end-developer-handbook-2019:
    parent: Manual del desarrollador front-end (2019)
    weight: 3

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 3
---

Este capítulo desglosará y describirá ampliamente la práctica de la ingeniería de front-end comenzando con "Cómo se hacen los desarrolladores de front-end".

## 2.1 - Cómo se hacen los desarrolladores front-end

¿Cómo se convierte uno en desarrollador front-end? Bueno, es complicado. Solo considere esta hoja de ruta:

![Hoja de ruta del desarrollador](/courses/front-end-developer-handbook-2019/chapter2-1.png)

<div class="source">Fuente de la imagen: https://github.com/kamranahmedse/developer-roadmap</div>

Hoy en día, en general, uno no puede ir a la universidad y esperar graduarse con un título en ingeniería de front-end. Y, rara vez escucho o conozco a desarrolladores front-end que sufrieron lo que probablemente sea un título en ciencias de la computación obsoleto o un título en diseño gráfico para terminar escribiendo HTML, CSS y JavaScript profesionalmente. Desde mi perspectiva, la mayoría de las personas que trabajan en el front-end hoy en día generalmente parecen ser autodidactas desde cero o cruzar al espacio del front-end desde los campos del diseño o la informática.

Si hoy se dispusiera a convertirse en un desarrollador front-end, me esforzaría en seguir el proceso que se describe a continuación (el Capítulo 3 y el Capítulo 4 profundizarán en más detalles sobre los recursos de aprendizaje).

1. Aprenda, aproximadamente, cómo funciona la [plataforma](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/How_does_the_Internet_work) [web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works). Asegúrese de conocer el "qué" y el "dónde" de [HTML, CSS, DOM, JavaScript, dominios, DNS, URL, HTTP, navegadores y servidores/alojamiento](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web). No profundice en nada todavía, solo intente comprender las partes en juego y cómo encajan libremente. Empiece por crear páginas web sencillas.
2. [Aprenda HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML)
3. [Aprenda CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)
4. [Aprenda JavaScript](https://youtu.be/QjKH1J77gjI?list=PL055Epbe6d5bQubu5EWf_kUNA3ef_qbmL)
5. Aprenda DOM
6. Aprenda los fundamentos del diseño de la interfaz de usuario (es decir, patrones de interfaz de usuario, diseño de interacción, diseño de experiencia de usuario y usabilidad).
7. Aprenda CLI / línea de comandos
8. Aprenda la práctica de la ingeniería de software (es decir, diseño / arquitectura de aplicaciones, plantillas, Git, pruebas, monitoreo, automatización, calidad del código, metodologías de desarrollo).
9. Sea obstinado y personalice su caja de herramientas con lo que tenga sentido para su cerebro (por ejemplo, Webpack, React y Mobx).
10. Aprenda Node.js

Un breve consejo sobre el aprendizaje. [Aprenda las tecnologías subyacentes reales, antes de aprender abstracciones](https://youtu.be/QjKH1J77gjI?list=PL055Epbe6d5bQubu5EWf_kUNA3ef_qbmL). No aprenda jQuery, aprenda el DOM. No aprenda SASS, aprenda CSS. No aprenda JSX, aprenda HTML. No aprenda TypeScript, aprenda JavaScript. No aprenda Handlebars, aprenda las plantillas JavaScript ES6. No solo use Bootstrap, aprenda patrones de interfaz de usuario.

Últimamente han surgido muchas escuelas / bootcamps de código front-end no acreditados y costosos. Estas vías para convertirse en un desarrollador front-end suelen ser cursos dirigidos por maestros, que siguen un estilo de aprendizaje más tradicional, de un instructor oficial (es decir, programa de estudios, pruebas, cuestionarios, proyectos, proyectos de equipo, calificaciones, etc.).

Tenga en cuenta que si está considerando un programa de capacitación costoso, ¡esta es la web!
Todo lo que necesita aprender está disponible en la web y cuesta poco o nada.

Sin embargo, si necesita que alguien le diga cómo tomar y aprender qué es de bajo costo a gratis, y lo responsabilice por aprenderlo, debe considerar un salón de clase tradicional dirigido por un instructor. De lo contrario, no conozco ninguna otra profesión que sea prácticamente gratuita para tomar con una conexión a Internet, [un par de dólares al mes para membresías de screencasting](https://frontendmasters.com/join/) y un deseo ardiente de conocimiento.

Por ejemplo, si desea comenzar hoy, consumir uno o más de los siguientes recursos autodirigidos a continuación puede funcionar:

- [Introducción a la Web](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web) [leer]
- [Entonces, quieres ser un ingeniero de front-end](https://www.youtube.com/watch?v=Lsg84NtJbmI) [ver]
- [Rutas de aprendizaje de Frontend Masters](https://frontendmasters.com/learn) [ver] [$]
- [Introducción al desarrollo web](https://frontendmasters.com/courses/web-development-v2/) [ver] [$]
- [Título técnico de Treehouse](https://teamtreehouse.com/techdegree/front-end-web-development-2) [ver] [$]
- [Nanodegree de desarrollador web front-end](https://www.udacity.com/course/front-end-web-developer-nanodegree--nd001) [ver] [$]
- [Conviértase en desarrollador web front-end](https://www.lynda.com/learning-paths/Web/become-a-front-end-web-developer) [ver] [$]
- [freeCodeCamp](https://learn.freecodecamp.org/) [interactivo] [ver]

Al comenzar, debe temer la mayoría de las cosas que ocultan complejidad. Las abstracciones (por ejemplo, jQuery) en las manos equivocadas pueden dar la apariencia de habilidades avanzadas, mientras que todo el tiempo ocultan el hecho de que un desarrollador tiene una comprensión inferior de los conceptos básicos o subyacentes.

Se supone que en este viaje no solo está aprendiendo, sino también haciendo a medida que aprende e investiga herramientas. Algunos sugieren solo hacer para aprender. Mientras que otros sugieren solo aprender a hacer. Le sugiero que busque una combinación de ambos que coincida con el funcionamiento de su cerebro y haga eso. Pero, seguro, ¡es una mezcla! Por lo tanto, no se limite a leer sobre ello, hágalo. Aprende, haz. Aprende, haz. Repita indefinidamente porque las cosas cambian rápido. Por eso es tan importante aprender los fundamentos y no las abstracciones.

## 2.2 - Títulos de trabajo de front-end

[Durante varios años se ha estado gestando una gran división en el espacio del desarrollador front-end entre dos tipos muy diferentes de los denominados desarrolladores front-end](https://css-tricks.com/the-great-divide/). Por un lado, tiene programadores centrados en JavaScript que escriben JavaScript para tiempos de ejecución de front-end que probablemente tengan habilidades en informática con un historial de desarrollo de software. Lo más probable es que vean HTML y CSS como una abstracción (es decir, [JSX](https://reactjs.org/docs/introducing-jsx.html) y [CSS en JS](https://hackernoon.com/all-you-need-to-know-about-css-in-js-984a72d48ebc)). Por otro lado, lo más probable es que tenga desarrolladores sin formación en informática que se centran en HTML, CSS y JavaScript en lo que respecta específicamente a la interfaz de usuario. En 2019, cuando ingrese o intente comprender el espacio del desarrollador de front-end, sentirá absolutamente esta división. El término desarrollador front-end está al borde de la falta de significado sin aclarar las palabras para abordar qué tipo de desarrollador front-end se está discutiendo.

A continuación se muestra una lista y descripción de varios títulos de trabajo de front-end (tenga en cuenta que los títulos son [difíciles](https://blog.prototypr.io/dissecting-front-end-job-titles-7f72a0ef0bc5)). El título más común o más utilizado (es decir, genérico) para un desarrollador front-end es "desarrollador front-end" o "ingeniero front-end". Tenga en cuenta que cualquier trabajo que contenga la palabra "interfaz", "lado del cliente", "interfaz de usuario web", "HTML", "CSS" o "JavaScript" normalmente implica que la persona tiene cierto grado de conocimientos profesionales de HTML, CSS, DOM y JavaScript.

**Desarrollador front-end**: el título de trabajo genérico que describe a un desarrollador que tiene alguna habilidad en HTML, CSS, DOM y JavaScript y que implementa estas tecnologías en la plataforma web.

**Ingeniero de front-end (también conocido como desarrollador de JavaScript o desarrollador JavaScript de pila completa)**: el título de trabajo otorgado a un desarrollador que proviene de una experiencia en ciencias de la computación, ingeniería, y que usa estas habilidades para trabajar con tecnologías frontales. Esta función normalmente requiere conocimientos de informática y años de experiencia en desarrollo de software. Cuando se incluye la palabra "Aplicación JavaScript" en el título del trabajo, esto indicará que el desarrollador debe ser un avanzado
Desarrollador de JavaScript que posee habilidades avanzadas de programación, desarrollo de software y desarrollo de aplicaciones (es decir, tiene años de experiencia en la creación de aplicaciones de software front-end).

**Desarrollador CSS / HTML**: el título de trabajo de front-end que describe a un desarrollador que tiene conocimientos de HTML y CSS, excluyendo JavaScript y aplicaciones.

**Diseñador web front-end**: cuando se incluye la palabra "Diseñador" en el título del trabajo, esto indicará que el diseñador poseerá habilidades front-end (es decir, HTML y CSS) pero también habilidades de diseño profesional (diseño visual y diseño de interacción).

**Desarrollador / ingeniero de UI (interfaz de usuario)**: cuando la palabra "Interfaz" o "UI" se incluye en el título del trabajo, esto indicará que el desarrollador debe poseer habilidades de diseño de interacción además de habilidades de desarrollador front-end o ingeniería front-end.

**Desarrollador front-end móvil / tablet**: cuando se incluye la palabra "Móvil" o "Tablet" en el título del trabajo, esto indicará que el desarrollador tiene experiencia en el desarrollo de interfaces que se ejecutan en dispositivos móviles o tabletas (ya sea de forma nativa o en plataforma web, es decir, en un navegador).

**Experto en SEO de Front-End**: Cuando la palabra "SEO" se incluye en el título del trabajo, esto indicará que el desarrollador tiene una amplia experiencia en la elaboración de tecnologías de front-end hacia una estrategia de SEO.

**Experto en accesibilidad de front-end**: cuando se incluye la palabra "Accesibilidad" en el título del trabajo, esto indicará que el desarrollador tiene una amplia experiencia en la elaboración de tecnologías de front-end que respaldan los requisitos y estándares de accesibilidad.

**Desarrollo front-end Dev.Ops**: cuando se incluye la palabra "DevOps" en el título del trabajo, esto indicará que el desarrollador tiene una amplia experiencia con las prácticas de desarrollo de software relacionadas con la colaboración, integración, implementación, automatización y calidad.

**Pruebas de front-end / QA**: cuando la palabra "Testing" o "QA" se incluye en el título del trabajo, esto indicará que el desarrollador tiene una amplia experiencia probando y administrando software que involucra pruebas unitarias, pruebas funcionales, pruebas de usuario y Pruebas A/B.

> Notas:<br>  
Si encuentra los términos "Full Stack" o los términos genéricos "Web Developer" en los títulos de trabajo, estas palabras pueden ser utilizadas por un empleador para describir una función que es responsable de todos los aspectos del desarrollo web / de aplicaciones, es decir, tanto de front-end (potencialmente incluyendo diseño) y back-end.

## 2.3 - Tecnologías web de referencia empleadas por desarrolladores front-end

![Tenologías web](/courses/front-end-developer-handbook-2019/chapter2-7.png)

Las siguientes tecnologías web centrales son empleadas por desarrolladores front-end (considere aprenderlas en este orden):

1. Lenguaje de marcado de hipertexto (también conocido como HTML)
2. Hojas de estilo en cascada (también conocidas como CSS)
3. Localizadores uniformes de recursos (también conocidos como URL)
4. Protocolo de transferencia de hipertexto (también conocido como HTTP)
5. Lenguaje de programación JavaScript (también conocido como ECMAScript 262)
6. Notación de objetos JavaScript (también conocida como JSON)
7. Modelo de objeto de documento (también conocido como DOM)
8. API web (también conocidas como HTML5 and friends o API del navegador)
9. Pautas de accesibilidad al contenido web (también conocidas como WCAG) y Aplicaciones de Internet enriquecido accesible

Para obtener una lista completa de todas las especificaciones relacionadas con la web, consulte [platform.html5.org](https://platform.html5.org/) o las [API web de MDN](https://developer.mozilla.org/en-US/docs/Web/API).

Las nueve tecnologías que se acaban de mencionar se definen a continuación junto con un enlace a la documentación y especificaciones relevantes para cada tecnología.

### Lenguaje de marcado de hipertexto (también conocido como HTML)

> El lenguaje de marcado de hipertexto, comúnmente conocido como HTML, es el lenguaje de marcado estándar utilizado para crear páginas web. HTML describe la estructura de un sitio web semánticamente junto con pistas para la presentación, lo que lo convierte en un lenguaje de marcado, en lugar de un lenguaje de programación.<br>  
<div class="source">- Wikipedia</div>

Especificaciones / documentación más relevantes:

- [Todas las especificaciones HTML del W3C](http://www.w3.org/standards/techs/html#w3c_all)
- [Los elementos de HTML](https://html.spec.whatwg.org/multipage) de Living Standard
- [Atributos globales](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes)
- [HTML 5.2 de W3C](https://www.w3.org/TR/2017/REC-html52-20171214/)
- [HTML 5.3 de W3C](http://w3c.github.io/html/)
- [Referencia de atributo HTML](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes)
- [Referencia de elemento HTML](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
- [La sintaxis HTML](https://html.spec.whatwg.org/multipage/syntax.html#syntax) de Living Standard

### Hojas de estilo en cascada (también conocidas como CSS)

> Hojas de estilo en cascada (CSS) es un lenguaje de hojas de estilo que se utiliza para describir el aspecto y el formato de un documento escrito en un lenguaje de marcado. Aunque se utiliza con mayor frecuencia para cambiar el estilo de las páginas web y las interfaces de usuario escritas en HTML y XHTML, el lenguaje se puede aplicar a cualquier tipo de documento XML, incluidos XML simple, SVG y XUL. Junto con HTML y JavaScript, CSS es una tecnología fundamental utilizada por la mayoría de los sitios web para crear páginas web visualmente atractivas, interfaces de usuario para aplicaciones web e interfaces de usuario para muchas aplicaciones móviles.<br>  
<div class="source">- Wikipedia</div>

Especificaciones / documentación más relevantes:

- [Todas las especificaciones CSS del W3C](http://www.w3.org/Style/CSS/current-work)
- [Especificación de hojas de estilo en cascada Nivel 2 Revisión 2 (CSS 2.2)](https://www.w3.org/TR/CSS22/)
- [Referencia CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)
- [Selectores Nivel 3](http://www.w3.org/TR/css3-selectors/)

### Protocolo de transferencia de hipertexto (también conocido como HTTP)

> El Protocolo de transferencia de hipertexto (HTTP) es un protocolo de aplicación para sistemas de información distribuidos, colaborativos e hipermedia. HTTP es la base de la comunicación de datos para la World Wide Web.<br>  
<div class="source">- Wikipedia</div>

Especificaciones más relevantes:

- [Protocolo de transferencia de hipertexto - HTTP / 1.1](https://tools.ietf.org/html/rfc2616)
- [HTTP / 2](http://httpwg.org/specs/rfc7540.html)

### Localizadores uniformes de recursos (también conocidos como URL)

> Un localizador uniforme de recursos (URL) (también llamado dirección web) es una referencia a un recurso que especifica la ubicación del recurso en una red informática y un mecanismo para recuperarlo. Una URL es un tipo específico de identificador uniforme de recursos (URI), aunque muchas personas usan los dos términos indistintamente. Una URL implica los medios para acceder a un recurso indicado, lo que no es cierto para todos los URI. Las URL ocurren con mayor frecuencia para hacer referencia a páginas web (http), pero también se utilizan para transferencia de archivos (ftp), correo electrónico (mailto), acceso a bases de datos (JDBC) y muchas otras aplicaciones.<br>  
<div class="source">- Wikipedia</div>

Especificaciones más relevantes:

- [Localizadores uniformes de recursos (URL)](http://www.w3.org/Addressing/URL/url-spec.txt)
- [Estándar de vida URL](https://url.spec.whatwg.org/)

### Modelo de objeto de documento (también conocido como DOM)

> El Document Object Model (DOM) es multiplataforma y una convención independiente del lenguaje para representar e interactuar con objetos en documentos HTML, XHTML y XML. Los nodos de cada documento están organizados en una estructura de árbol, llamada árbol DOM. Los objetos en el árbol DOM se pueden direccionar y manipular utilizando métodos en los objetos. La interfaz pública de un DOM se especifica en su interfaz de programación de aplicaciones (API).<br>  
<div class="source">- Wikipedia</div>

Especificaciones / documentación más relevantes:

- [Estándar de vida DOM](https://dom.spec.whatwg.org/)
- [W3C DOM4](https://www.w3.org/TR/domcore/)
- [Eventos de UI](https://www.w3.org/TR/uievents/)

### Lenguaje de programación JavaScript (también conocido como ECMAScript 262)

> JavaScript es un lenguaje de programación de alto nivel, dinámico, sin tipo e interpretado. Se ha estandarizado en la especificación del lenguaje ECMAScript. Junto con HTML y CSS, es una de las tres tecnologías esenciales de la producción de contenido en la World Wide Web; la mayoría de los sitios web lo utilizan y es compatible con todos los navegadores web modernos sin complementos. JavaScript está basado en prototipos con funciones de primera clase, lo que lo convierte en un lenguaje de múltiples paradigmas, que admite estilos de programación orientados a objetos, imperativos y funcionales. Tiene una API para trabajar con texto, matrices, fechas y expresiones regulares, pero no incluye ninguna E/S, como redes, almacenamiento o instalaciones de gráficos, confiando para estos en el entorno host en el que está integrado.<br>  
<div class="source">- Wikipedia</div>

Especificaciones / documentación más relevantes:

- [Especificación de idioma ECMAScript® 2018](http://ecma-international.org/ecma-262/9.0/index.html#Title)
- [Todas las especificaciones del lenguaje ECMAScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Language_Resources)

### API web (también conocidas como HTML5 y amigos)

> Al escribir código para la Web usando JavaScript, hay muchas API disponibles. A continuación se muestra una lista de todas las interfaces (es decir, tipos de objetos) que puede utilizar mientras desarrolla su sitio o aplicación web.<br>  
<div class="source">- Mozilla</div>

Documentación más relevante:

- [Interfaces API web](https://developer.mozilla.org/en-US/docs/Web/API)

### Notación de objetos JavaScript (también conocida como JSON)

> Es el formato de datos principal utilizado para la comunicación asíncrona entre navegador y servidor (AJAJ), que reemplaza en gran medida al XML (utilizado por AJAX). Aunque originalmente se deriva del lenguaje de secuencias de comandos de JavaScript, JSON es un formato de datos independiente del lenguaje. El código para analizar y generar datos JSON está disponible en muchos lenguajes de programación. El formato JSON fue especificado originalmente por Douglas Crockford. Actualmente está descrito por dos estándares competidores, RFC 7159 y ECMA-404. El estándar ECMA es mínimo, y describe solo la sintaxis gramatical permitida, mientras que el RFC también proporciona algunas consideraciones semánticas y de seguridad. El tipo de medio oficial de Internet para JSON es application/json. La extensión del nombre de archivo JSON es .json.<br>  
<div class="source">- Wikipedia</div>

Especificaciones más relevantes:

- [Presentamos JSON](http://json.org/)
- [API JSON](http://jsonapi.org/)
- [El formato de intercambio de datos JSON](http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-404.pdf)

### Pautas de accesibilidad al contenido web (también conocidas como WCAG) y aplicaciones enriquecidas de Internet accesibles (también conocidas como ARIA)

> La accesibilidad se refiere al diseño de productos, dispositivos, servicios o entornos para personas con discapacidad. El concepto de diseño accesible garantiza tanto el "acceso directo" (es decir, sin asistencia) como el "acceso indirecto", lo que significa compatibilidad con la tecnología de asistencia de una persona (por ejemplo, lectores de pantalla de computadora).<br>  
<div class="source">- Wikipedia</div>

- [Iniciativa de accesibilidad web (WAI)](https://www.w3.org/WAI/standards-guidelines/)
- [Estado actual de las Pautas de accesibilidad al contenido web (WCAG)](http://www.w3.org/standards/techs/wcag#w3c_all)

## 2.4 - Habilidades potenciales del desarrollador de front-end

![Colage de habilidades](/courses/front-end-developer-handbook-2019/chapter2-2.png)

<div class="source">Fuente de la imagen: http://blog.naustud.io/2015/06/baseline-for-modern-front-end-developers.html</div>

Se asume un conocimiento básico a avanzado de HTML, CSS, DOM, JavaScript, HTTP / URL y navegadores web para cualquier tipo de rol de desarrollador de aplicaciones para usuario.

Más allá de las habilidades que acabamos de mencionar, un desarrollador front-end también podría tener habilidades específicas en uno o más de los siguientes:

- Sistemas de gestión de contenido (también conocido como CMS)
- Node.js
- Prueba entre navegadores
- Pruebas multiplataforma
- Examen de la unidad
- Pruebas entre dispositivos
- Accesibilidad / WAI-ARIA
- Optimización de motores de búsqueda (también conocido como SEO)
- Diseño de interacción o interfaz de usuario
- Experiencia de usuario
- Usabilidad
- Sistemas de comercio electrónico
- Sistemas de portal
- Wireframing
- Diseño CSS / Cuadrículas
- Manipulación DOM (por ejemplo, jQuery)
- Rendimiento web móvil
- Prueba de carga
- Pruebas de rendimiento
- Mejora progresiva / degradación elegante
- Control de versiones (por ejemplo, GIT)
- MVC / MVVM / MV *
- Programación funcional
- Formatos de datos (por ejemplo, JSON, XML)
- API de datos (por ejemplo, Restful API)
- Incorporación de fuentes web: Gráficos vectoriales escalables (también conocidos como SVG)
- Expresiones regulares
- Microdatos / Microformatos
- Ejecutores de tareas, herramientas de compilación, herramientas de automatización de procesos
- Diseño web adaptable
- Programación orientada a objetos
- Arquitectura de aplicación
- Módulos
- Gerentes de dependencia
- Gestores de paquetes
- Animación JavaScript
- Animación CSS
- Cuadros / Gráficos
- Widgets de interfaz de usuario
- Prueba de calidad del código
- Prueba de cobertura de código
- Análisis de complejidad del código
- Pruebas de integración
- Línea de comando / CLI
- Plantillas de estrategias
- Motores de plantillas
- Aplicaciones de una sola página
- Seguridad web / navegador
- Herramientas para desarrolladores de navegadores

## 2.5 - Los desarrolladores front-end desarrollan para ...

Un desarrollador de front-end crea HTML, CSS y JS que normalmente se ejecuta en la [plataforma web](http://tess.oconnor.cx/2009/05/what-the-web-platform-is) (por ejemplo, un navegador web) entregado desde uno de los siguientes sistemas operativos (también conocidos como SO):

- [Android](https://www.android.com/)
- [Chromium](https://www.chromium.org/chromium-os)
- [iOS](https://developer.apple.com/ios/)
- [OS X](https://www.apple.com/macos) (es decir, MacOS)
- [Ubuntu](https://www.ubuntu.com/) (u otro sabor Linux)
- [Windows](https://www.microsoft.com/en-us/windows)

Estos sistemas operativos normalmente se ejecutan en uno o más de los siguientes dispositivos:

- Computadora de escritorio
- Computadora portátil / netbook
- Teléfono móvil
- Tableta
- televisión
- Reloj
- Cosas (es decir, cualquier cosa que pueda imaginar, automóvil, refrigerador, luces, termostato, etc.)

![Número de dispositivos conectados a internet](/courses/front-end-developer-handbook-2019/chapter2-3.png)

<div class="source">Fuente de la imagen: https://www.enterpriseirregulars.com/104084/roundup-internet-things-forecasts-market-estimates-2015/</div>

En términos generales, las tecnologías front-end se pueden ejecutar en los sistemas operativos y dispositivos mencionados anteriormente utilizando los siguientes escenarios de plataforma web en tiempo de ejecución:

- Un navegador web (ejemplos: [Chrome, IE, Safari, Firefox](http://outdatedbrowser.com/en)).
- Un [navegador sin cabeza](https://en.wikipedia.org/wiki/Headless_browser) (ejemplos: [Chromium sin cabeza](https://chromium.googlesource.com/chromium/src/+/lkgr/headless/README.md)).
- Una pestaña de [WebView](http://developer.telerik.com/featured/what-is-a-webview/)/navegador (piense en [iframe](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe)) incrustada dentro de una aplicación nativa como un tiempo de ejecución con un puente a las API nativas. Las aplicaciones WebView suelen contener una interfaz de usuario construida a partir de tecnologías web. (es decir, HTML, CSS y JS). (ejemplos: [Apache Cordova](https://cordova.apache.org/), [NW.js](http://nwjs.io/), [Electron](http://electron.atom.io/))
- Una aplicación nativa construida a partir de tecnología web que se interpreta en tiempo de ejecución con un puente a las API nativas. La interfaz de usuario utilizará partes de la interfaz de usuario nativas (por ejemplo, controles nativos de iOS), no tecnologías web. (ejemplos: [NativeScript](https://www.nativescript.org/), [React Native](https://facebook.github.io/react-native/))

## 2.6 - Front-End en un equipo

Un desarrollador front-end suele ser solo un jugador en un equipo que diseña y desarrolla sitios web, aplicaciones web o aplicaciones nativas que se ejecutan desde tecnologías web.
Un equipo de desarrollo básico para la creación de sitios web profesionales o software para la plataforma web normalmente contendrá, como mínimo, las siguientes funciones:

- Diseñador visual (es decir, fuentes, colores, espaciado, emoción, conceptos visuales y temas)
- UI / Diseñador de interacciones / Arquitecto de información (es decir, wireframes, especificando todas las interacciones del usuario y la funcionalidad de la UI, estructurando la información)
- Desarrollador front-end (es decir, escribe código que se ejecuta en el cliente / en el dispositivo)
- Desarrollador back-end (es decir, escribe código que se ejecuta en el servidor)

Los roles se ordenan de acuerdo con habilidades superpuestas. Un desarrollador de front-end normalmente tendrá un buen manejo del diseño de UI / Interacción, así como del desarrollo de back-end. No es raro que los miembros del equipo llenen más de un rol asumiendo las responsabilidades de un rol superpuesto.

Se supone que el equipo mencionado anteriormente está siendo dirigido por un líder del proyecto o algún tipo de propietario del producto (es decir, un interesado, gerente de proyecto, líder del proyecto, etc.)

Un equipo web más grande podría incluir los siguientes roles que no se muestran arriba:

- Estrategas SEO
- Ingenieros de DevOps
- Ingenieros de rendimiento
- Desarrolladores de API
- Administradores de bases de datos Ingenieros / probadores de QA

## 2.7 - Mito generalista/de pila completa

![Desarrollador full stack](/courses/front-end-developer-handbook-2019/chapter2-4.png)

El término desarrollador "Full-Stack" ha adquirido varios significados. Tantos, que ningún significado queda claro cuando se usa el término. Solo considere los resultados de las dos encuestas que se muestran a continuación. Estos resultados pueden llevar a uno a creer que ser un desarrollador de pila completa es algo común. Pero, en mis casi 20 años de experiencia, este es todo menos el caso en un contexto profesional.

![Qué rol te interesa](/courses/front-end-developer-handbook-2019/chapter2-5.png)

<div class="source">Fuente de la imagen: https://medium.freecodecamp.com/we-asked-15-000-people-who-they-are-and-how-theyre-learning-to-code-4104e29b2781#.ngcpn8nlz</div>

![Tipo de desarrollador](/courses/front-end-developer-handbook-2019/chapter2-6.png)

<div class="source">Fuente de la imagen: https://insights.stackoverflow.com/survey/2017#developer-profile-specific-developer-types</div>

Los roles para diseñar y desarrollar un sitio web o una aplicación web requieren un conjunto profundo de habilidades y una vasta experiencia en el área de diseño visual, diseño de interfaz de usuario/interacción, [desarrollo front-end](https://github.com/kamranahmedse/developer-roadmap#-front-end-roadmap) y [desarrollo back-end](https://github.com/kamranahmedse/developer-roadmap#-back-end-roadmap). Cualquier persona que pueda desempeñar uno o más de estos 4 roles a nivel profesional es un bien extremadamente raro.

De manera pragmática, debe buscar ser, o buscar contratar, un experto en uno de estos roles (es decir, diseño visual, diseño de interacción/IA, desarrollo de front-end, desarrollador de back-end). Aquellos que afirman operar a un nivel experto en uno o más de estos roles son excepcionalmente raros.

Sin embargo, dado que JavaScript se ha infiltrado en todas las capas de una pila de tecnología (es decir, Node.js), encontrar un desarrollador de JS de pila completa que pueda codificar el front-end y el back-end se está volviendo menos mítico. Normalmente, estos desarrolladores de pila completa solo se ocupan de JavaScript. Un desarrollador que puede codificar el front-end, el back-end, la API y la base de datos no es tan absurdo como antes (excluyendo el diseño visual, el diseño de interacción y CSS). Sigue siendo mítico en mi opinión, pero no tan infrecuente como antes. Por lo tanto, no recomendaría a un desarrollador que se proponga convertirse en un desarrollador "full-stack". En raras situaciones, puede funcionar. Pero, como concepto general para desarrollar una carrera como desarrollador front-end, me centraría en las tecnologías front-end.

## 2.8 - Entrevistas front-end

### Preparando:

- [Preparación para una entrevista de desarrollo web front-end en 2017](http://davidshariff.com/blog/preparing-for-a-front-end-web-development-interview-in-2017/)
- [Rompiendo la entrevista de front-end](https://medium.freecodecamp.com/cracking-the-front-end-interview-9a34cd46237)
- [Manual de entrevistas de front-end](https://github.com/yangshun/front-end-interview-handbook)
- [Decodificación del proceso de entrevista de front-end](https://dev.to/emmawedekind/decoding-the-front-end-interview-process-14dl)

### Prueba:

- [Cuestionario de desarrollo web front-end](http://davidshariff.com/quiz/)
- [Cuestionario web de JavaScript](http://davidshariff.com/js-quiz/)

### Preguntas que le pueden hacer:

- [10 preguntas de la entrevista que todo desarrollador de JavaScript debe saber](https://medium.com/javascript-scene/10-interview-questions-every-javascript-developer-should-know-6fa6bdf5ad95)
- [Preguntas de la entrevista de trabajo front-end](http://h5bp.github.io/Front-end-Developer-Interview-Questions/)
- [Cuestionario de desarrollo web front-end](http://davidshariff.com/quiz/)
- [Preguntas de la entrevista para desarrolladores front-end](http://thatjsdude.com/interview/index.html)
- [Las mejores preguntas de la entrevista de JavaScript de frontend (escritas por un ingeniero de frontend)](https://performancejs.com/post/hde6d32/The-Best-Frontend-JavaScript-Interview-Questions-(Written-by-a-Frontend-Engineer)

### Preguntas que haces:

- [Una lista open source de preguntas de los desarrolladores para hacerles a los posibles empleadores](https://github.com/ChiperSoft/InterviewThis)

## 2.9 - Tableros de trabajos de front-end

Existe una plétora de salidas de listados de trabajos técnicos. La lista reducida a continuación son actualmente los recursos más relevantes para encontrar un puesto / carrera de front-end específico.

- [Authenticjobs.com](https://authenticjobs.com/#category=4)
- [careers.stackoverflow.com](http://careers.stackoverflow.com/jobs?searchTerm=front-end)
- [css-tricks.com/jobs](https://css-tricks.com/jobs/)
- [frontenddeveloperjob.com](http://frontenddeveloperjob.com/)
- [glassdoor.com](http://www.glassdoor.com/Job/front-end-developer-jobs-SRCH_KO0,19.htm?jobType=all)
- [jobs.github.comlinkedin.com](https://jobs.github.com/)
- [remote.co](https://remote.co/remote-jobs/developer/)
- [weworkremotely.com](https://weworkremotely.com/)
- [www.smashingmagazine.com/jobs/](https://www.smashingmagazine.com/jobs/)

> Notas:<br>  
Desea trabajar de forma remota como desarrollador front-end, consulte estas [empresas compatibles con el control remoto](https://github.com/jessicard/remote-jobs).

## 2.10 - Salarios iniciales

El promedio nacional en los EEUU para un desarrollador front-end de nivel medio está entre $ 65k y 100k.

Por supuesto, cuando comience por primera vez, espere ingresar al campo en alrededor de 40k, dependiendo de la ubicación y la experiencia.

>Notas:<br>  
Un desarrollador / ingeniero principal / principal de front-end puede potencialmente vivir donde quiera (es decir, trabajar de forma remota) y ganar más de $ 150 mil al año (visite [angel.co](https://angel.co/jobs), regístrese, revise trabajos de front-end de más de $ 150k o examine el salario rangos en [Stack Overflow Jobs](https://stackoverflow.com/jobs?q=front-end&sort=y)).
