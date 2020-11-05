---
title: Capítulo 0. Resumen de 2018 y análisis futuro
linktitle: Capítulo 0. Resumen de 2018 y análisis futuro
toc: true
type: docs
date: "2020-09-03T00:00:00+01:00"
draft: false
menu:
  front-end-developer-handbook-2019:
    parent: Manual del desarrollador front-end (2019)
    weight: 1

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 1
---


## 0.1 - Resumen del desarrollo front-end en 2018

- React tuvo varios lanzamientos notables el año pasado que incluyeron [métodos de ciclo de vida](https://reactjs.org/blog/2018/03/29/react-v-16-3.html#component-lifecycle-changes), [API de contexto](https://reactjs.org/blog/2018/03/29/react-v-16-3.html#official-context-api), [suspenso](https://reactjs.org/docs/react-api.html#reactsuspense) y [React hooks](https://reactjs.org/docs/hooks-intro.html).

- [Microsoft compra Github](https://news.microsoft.com/2018/06/04/microsoft-to-acquire-github-for-7-5-billion/). Sí, eso pasó.

- Las fuentes creadas por CSS se convirtieron en una [cosa](https://yusugomori.com/projects/css-sans/).

- Lo que solía llamar aplicaciones dirigidas por el front-end, se etiqueta como ["sin servidor"](https://thepowerofserverless.info/). Desafortunadamente, este término está [sobrecargado](https://frontendmasters.com/books/front-end-handbook/2019/owler.com/articles/serverless.html). Sin embargo, el término [JAMstack](https://jamstack.org/) parece estar [resonando](https://jamstackconf.com/nyc/) entre los desarrolladores.

- Google ofreció algunas herramientas interesantes este año para ayudar a que las páginas web se carguen más rápido, es decir, [squoosh](https://github.com/GoogleChromeLabs/squoosh/) y [quicklink](https://github.com/GoogleChromeLabs/quicklink).

- [Vue](https://risingstars.js.org/2018/en/#section-framework) obtiene más [estrellas de Github](https://hasvuepassedreactyet.surge.sh/) que React este año. Pero React sigue siendo dominante en [términos](https://2018.stateofjs.com/front-end-frameworks/overview/) de [uso](https://www.npmjs.com/browse/depended).

- Se introduce una solución similar a React, sin un DOM virtual o JSX, [RE:DOM](https://github.com/redom/redom).

- Aparecen alternativas a NW.js y Electron, [DeskGap](https://deskgap.com/) y [Neutralino.js](https://neutralino.js.org/).

- En 2017, la [gran división](https://medium.com/@jerrylowm/the-death-of-front-end-developers-803a95e0f411) entre un [desarrollador front-end HTML y CSS](https://medium.com/@mandy.michael/is-there-any-value-in-people-who-cannot-write-javascript-d0a66b16de06) vs el [desarrollador de aplicaciones front-end se realiza/verbaliza](https://css-tricks.com/the-great-divide/). En 2018, esa [división se ha hecho más y más profunda](https://css-tricks.com/the-great-divide/) y más [personas](https://rachelandrew.co.uk/archives/2019/01/30/html-css-and-our-vanishing-industry-entry-points/) comienzan a [sentirla](https://justmarkup.com/log/2018/11/just-markup/).

- Este año, como los años más recientes, estuvo lleno de soluciones de aplicaciones/frameworks que intentaban competir con las principales herramientas de aplicaciones de JavaScript (es decir, [React, Angular y Vue, etc](https://stateofjs.com/2017/front-end/results)) Permítame enumerarlas para usted: [Radi.js](https://radi.js.org/), [DisplayJS](https://display.js.org/), [Stimulus](https://stimulusjs.org/), [Omi](https://github.com/Tencent/omi), [Quasar](https://quasar-framework.org/).

- Los frameworks de JavaScript comienzan a ofrecer sus propios lenguajes que se compilan en JavaScript (por ejemplo, [Mint](https://www.mint-lang.com/)).

- [CodeSandbox](https://codesandbox.io/) evoluciona para convertirse en la solución dominante para compartir código en línea.

- [CSS Grid](https://cssgridgarden.com/) y [CSS Flexbox](https://flexboxfroggy.com/) son totalmente compatibles con los navegadores modernos y se toman en serio. Pero [muchos se preguntan](https://www.youtube.com/watch?v=hs3piaN4b5I) cuándo [usar cuál y cómo](https://css-irl.info/to-grid-or-to-flex/).

- Muchos se dan cuenta de los costos a largo plazo de los sistemas de tipos atornillados (por ejemplo, TypeScript y Flow). Algunos concluyeron que los sistemas atornillados no son diferentes a los sistemas atornillados en módulos (es decir, AMD/Require.js) y vienen con [más problemas que soluciones](https://medium.com/javascript-scene/the-typescript-tax-132ff4cb175b). Como mínimo, muchos desarrolladores se dan cuenta de que si se necesitan tipos en grandes bases de código, los sistemas atornillados no son ideales en comparación con los lenguajes que los tienen integrados (por ejemplo, [Reason](https://reasonml.github.io/), [Purescript](http://www.purescript.org/), [Elm](https://elm-lang.org/)).

- Las [variables CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_variables) obtienen [soporte de navegador](https://caniuse.com/#feat=css-variables) entre los navegadores web modernos.

- Los sabores de [CSS en JS](http://michelebertoli.github.io/css-in-js/) explotaron y [algunos cuestionan](http://bradfrost.com/blog/link/whats-wrong-with-css-in-js/) la práctica.

- Los [módulos ES](https://caniuse.com/#search=modules) ahora se pueden utilizar en navegadores modernos y las [importaciones dinámicas](https://developers.google.com/web/updates/2017/11/dynamic-import#dynamic)
están muy cerca. Incluso estamos viendo un cambio en las [herramientas](https://www.pikapkg.com/blog/introducing-pika-pack/) en torno a este hecho.

- Muchos se dan cuenta de que las pruebas de extremo a extremo son el punto de partida para realizar las pruebas correctamente en gran parte debido a [Cypress](https://www.cypress.io/how-it-works/) (es decir, Cypress primero, luego [Jest](https://jestjs.io/)).

- Si bien [Webpack](https://webpack.js.org/) se usó mucho nuevamente este año, muchos desarrolladores encontraron que [Parcel](https://github.com/parcel-bundler/parcel) era más fácil de configurar y ejecutar.

- Una de las preguntas más importantes que se hicieron este año fue cuál es el [costo de JavaScript](https://medium.com/@addyosmani/the-cost-of-javascript-in-2018-7d8950fbb5d4).

- [Babel 7 fue lanzado este año](https://babeljs.io/blog/2018/08/27/7.0.0). Eso es un gran problema porque la última versión importante fue hace casi tres años.

- La realidad de muchos cambios de JavaScript demasiado rápido se hace realidad y la [gente comienza a hablar](https://www.robinwieruch.de/javascript-fundamentals-react-requirements/) sobre lo que necesita saber antes de que pueda aprender algo como React. La pelea es real.

- La mayoría de los desarrolladores encontraron GraphQL, a través de [Apollo](https://www.apollographql.com/), y [lo ven](https://blog.bitsrc.io/why-does-everyone-love-graphql-17de7f99f05a) como la próxima evolución para las API de datos.

- Gulp y sus amigos definitivamente pasaron a un segundo plano en la [ejecución de NPM/Yarn](https://css-tricks.com/why-npm-scripts/). Pero esto no impidió que Microsoft entrara en el juego con [Just](https://github.com/Microsoft/just).

- Este año, no solo se puede hilar/insinuar HTML, CSS y JavaScript, sino que también se puede [hilar/insinuar la web misma](https://webhint.io/).

- Vale la pena leer la [encuesta de 2018 Front-End Tooling](https://ashleynolan.co.uk/blog/frontend-tooling-survey-2018-results), aunque solo sea para darse cuenta de cuánto jQuery todavía se usa.

- [No se puede negar](https://2018.stateofjs.com/javascript-flavors/typescript/) que [TypeScript](https://www.typescriptlang.org/) ganó muchos usuarios este año.

- [VScode](https://code.visualstudio.com/), [domina](https://triplebyte.com/blog/editor-report-the-rise-of-visual-studio-code) como el editor de código de elección.

## 0.2 - En 2019, espere ...

- Con suerte, más de esto por venir. "[Alejándose de Sass](https://cathydutton.co.uk/posts/why-i-stopped-using-sass/)".

- Sigue siendo una buena idea para estar atento y conocer las próximas adiciones (y posibles adiciones) a CSS a través de https://cssdb.org

- El formato de imagen [WebP](https://developers.google.com/speed/webp/) de Google podría alcanzar el [soporte de todos los navegadores modernos](https://caniuse.com/#feat=webp) este año.

- [Prepack](https://prepack.io/) seguirá cocinando.

- [GraphQL](https://graphql.org/) seguirá ganando una adopción masiva.

- Los autores de la encuesta "[Estado de JavaScript](https://stateofjs.com/)" agregarán una encuesta de "[Estado de CSS](https://stateofcss.com/)" en 2019.

- Esté atento a la [API de animaciones web](https://caniuse.com/#feat=web-animation).

- Alguien que conoces intentará convencerte de que utilices [TypeScript](https://www.typescriptlang.org/).

- Babel obtendrá algo de competencia de [swc-project](https://github.com/swc-project/swc).

- El caso de [JAMStack](https://jamstack.org/) [continuará](https://jamstackconf.com/nyc/).

- [Continuará la búsqueda de una base de código para muchas plataformas](https://quasar-framework.org/).

- Más desarrolladores recurrirán a lenguajes como [ReasonML](https://www.imaginarycloud.com/blog/reasonml-react-as-first-intended/) sobre JavaScript/TypeScript para bases de código grandes.

- Los [proyectos más utilizados](https://github.com/twbs/bootstrap/pull/23586) comenzarán a deshacerse de jQuery a favor de las soluciones DOM nativas.

- [Componentes web](https://developer.mozilla.org/en-US/docs/Web/Web_Components)! En este punto, no tengo idea de cómo funcionarán los componentes web. La realidad es que no se van a ir y no han ganado mucho impulso/ uso una vez que terminó el bombo.
