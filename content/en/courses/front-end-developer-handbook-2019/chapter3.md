---
title: Chapter 3. Learning Front-end Dev. SelfDirected Resources/Recommendations
linktitle: Chapter 3. Learning Front-end Dev. SelfDirected Resources/Recommendations
toc: true
type: docs
date: "2020-09-03T00:00:00+01:00"
draft: false
menu:
  front-end-developer-handbook-2019:
    parent: Front end developer handbook 2019
    weight: 4

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 4
---

This chapter highlights the many resources (video training, books, etc.) that an individual can use to direct their own learning process and career as a front-end developer.
The learning resources identified (articles, books, videos, screencasts etc..) will include both free and paid material. Paid material will be indicated with [$].
3.1. - Learn Internet/Web
The Internet is a global system of interconnected computer networks that use the Internet protocol suite (TCP/IP) to link several billion devices worldwide. It is a network of networks that consists of millions of private, public, academic, business, and government networks of local to global scope, linked by a broad array of electronic, wireless, and optical networking technologies. The Internet carries an extensive range of information resources and services, such as the inter-linked hypertext documents and applications of the World Wide Web (WWW), electronic mail, telephony, and peer-to-peer networks for file sharing.
— WikipediaImage source: https://www.helloitsliam.com/2014/12/20/how-the-internet-works-infographic/
What is the Internet? [watch]
Internet Fundamentals [watch]
How the Web works [read]
How does the Internet work? https://developer.mozilla.org/en-
US/docs/Learn/Common_questions/How_does_the_Internet_work and http://web.stanford.edu/class/msande91si/www-
spr04/readings/week1/InternetWhitepaper.htm [read]
How the Internet Works [watch]
How the Internet Works in 5 Minutes [watch]
How the Web Works [watch]
What Is the Internet? Or, "You Say Tomato, I Say TCP/IP" [read]
Donʼt Fear the InternetImage source: http://www.bitrebels.com/technology/find-out-who-runs-the-internet-chart/
3.2. - Learn Web Browsers
A web browser (commonly referred to as a browser) is a software application for retrieving, presenting, and traversing information resources on the World Wide Web. An information resource is identified by a Uniform Resource Identifier (URI/URL) and may be a web page, image, video or other piece of content. Hyperlinks present in resources enable users easily to navigate their browsers to related resources.Although browsers are primarily intended to use the World Wide Web, they can also be used to access information provided by web servers in private networks or files in file systems.
— Wikipedia
The most commonly used browsers (on desktop and mobile) are:
l. Chrome (engine: Blink + V8)
n. Firefox (engine: Gecko + SpiderMonkey)
o. Internet Explorer (engine: Trident + Chakra)
p. Safari (engine: Webkit + SquirrelFish)
Image source: http://gs.statcounter.com/browser-market-share
Evolution of Browsers & Web Technologies (i.e., APIs)
evolutionoftheweb.com [read]Timeline of web browsers [read]
The Most Commonly Used Headless Browser Are:
Headless Chromium (engine: Blink + V8)
SlimerJS (engine: Gecko + SpiderMonkey)
How Browsers Work
20 Things I Learned About Browsers and the Web [read]
Fast CSS: How Browsers Lay Out Web Pages [read]
How Browsers Work: Behind the scenes of modern web browsers [read]
Quantum Up Close: What is a browser engine?
So How Does the Browser Actually Render a Website [watch]
What forces layout / reflow [read]
What Every Frontend Developer Should Know About Webpage Rendering [read]
Optimizing for Browsers:
Browser Rendering Optimization [watch]
Website Performance Optimization [watch]
Comparing Browsers
Comparison of Web Browsers [read]
Browser Hacks
browserhacks.com [read]
Developing for Browsers
In the past, front-end developers spent a lot of time making code work
in severaldifferent browsers. This was once a bigger issue than it is today. Today, abstractions (e.g., React, Webpack, Post-CSS, Babel etc...) combined with modern browsers make browser development fairly easy. The new challenge is not which browser the user will use, but on which device they will run the browser.
Evergreen Browsers
The latest versions of most modern browsers are considered evergreen browsers.
That is, in theory, they are supposed to automatically update themselves silently without prompting the user. This move towards self-updating browsers has been in reaction to the slow process of eliminating older browsers that do not auto-update.
Picking a Browser
As of today, most front-end developers use Chrome and "Chrome Dev Tools" to develop front-end code. However, the most used modern browsers all offer a flavor of developer tools. Picking one to use for development is a subjective choice. The more important issue is knowing which browsers, on which devices, you have to support and then testing appropriately.
3.3 - Learn Domain Name System (aka DNS)

The Domain Name System (DNS) is a hierarchical distributed naming system for computers, services, or any resource connected to the Internet or a private network. It associates various information with domain names assigned to each of the participating entities. Most prominently, it translates domain names, which can be easilymemorized by humans, to the numerical IP addresses needed for the purpose of computer services and devices worldwide. The Domain Name System is an essential component of the functionality of most Internet services because it is the Internet's primary directory service.
— Wikipedia
Image source: http://www.digital-digest.com/blog/DVDGuy/wp-content/uploads/2011/11/how_dns_works.jpg
An Introduction to DNS Terminology, Components, and Concepts [read]
DNS Explained [watch]
How DNS Works [read]The Internet: IP Addresses and DNS [watch]
What is a domain name? [read]
3.4 - Learn HTTP/Networks (Including CORS & WebSockets)
HTTP - The Hypertext Transfer Protocol (HTTP) is an application protocol for distributed, collaborative, hypermedia information systems. HTTP is the foundation of data communication for the World Wide Web.
— Wikipedia
HTTP Specifications
HTTP/2
Hypertext Transfer Protocol -- HTTP/1.1
HTTP Docs
MDN HTTP [read]
HTTP Videos/Articles/Tutorials
High Performance Browser Networking: What Every Web Developer Should Know
About Networking and Web Performance [read]MDN: An overview of HTTP [read]
HTTP: The Definitive Guide (Definitive Guides) [read][$]
HTTP/2 Frequently Asked Questions [read]
HTTP Fundamentals [watch][$]
HTTP/2 Fundamentals [watch][$]
HTTP: The Protocol Every Web Developer Must Know - Part 1 [read]
HTTP: The Protocol Every Web Developer Must Know - Part 2 [read]
HTTP Succinctly [read]
HTTP Status Codes
HTTP Status Codes
HTTP Status Codes in 60 Seconds [watch]
CORS - Cross-origin resource sharing (CORS) is a mechanism that allows restricted resources (e.g., fonts) on a web page to be requested from another domain outside the domain from which the resource originated.
— Wikipedia
CORS Specifications
Cross-Origin Resource Sharing
CORSCORS in Action [read][$]
HTTP Access Control (CORS) [read]
WebSockets - WebSocket is a protocol providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C.
— Wikipedia
WebSockets
Connect the Web With WebSockets [watch]
WebSocket: Lightweight Client-Server Communications [read][$]
The WebSocket Protocol [read]
3.5 - Learn Web Hosting
A web hosting service is a type of Internet hosting service that allows individuals and organizations to make their website accessible via the World Wide Web. Web hosts are companies that provide space on a server owned or leased for use by clients, as well as providing Internetconnectivity, typically in a data center.
— Wikipedia
General Learning:
Web Hosting 101: Get Your Website Live on the Web in No Time [video]Image source: https://firstsiteguide.com/wp-content/uploads/2016/06/what-is-web-hosting-infographic.jpg
3.6 - Learn General Front-End Development
Frontend Bootcamp / Days in the Web [read]
Becoming a Career-Ready Web Developer
Become a Front-End Web Developer [watch][$]
Being a web developer [read]
freeCodeCamp [interact]
learning front-end development during #100DaysOfCode [read]
Front-End Web Developer Nanodegree [watch][$]
Front End Web Development Career Kickstart [watch][$]
Front End Web Development: Get Started [watch][$]
Front-End Web Development Quick Start With HTML5, CSS, and JavaScript [watch] [$]
Front-End Web Development: The Big Nerd Ranch Guide [read][$]
Complete Intro to Web Development [watch][$]
Learn Front End Web Development [watch][$]
So, You Want to Be a Front-End Engineer [watch]codecademy.com: Web Development Path [interact][free to $]
web.dev [read]
3.7 - Learn User Interface/Interaction Design
User Interface Design - User interface design (UI) or user interface engineering is the design of user interfaces for machines and software, such as computers, home appliances, mobile devices, and other electronic devices, with the focus on maximizing the user experience.
The goal of user interface design is to make the user's interaction as simple and efficient as possible, in terms of accomplishing user goals (user-centered design).
— Wikipedia
Interaction Design Pattern - A design pattern is a formal way of documenting a solution to a common design problem. The idea was introduced by the architect Christopher Alexander for use in urban planning and building architecture, and has been adapted for various other disciplines, including teaching and pedagogy, development organization and process, and software architecture and design.
— Wikipedia
User Experience Design - User Experience Design (UXD or UED or XD) is the process of enhancing user satisfaction by improving the usability, accessibility, and pleasure provided in the interaction between the userand the product. User experience design encompasses traditional human–computer interaction (HCI) design, and extends it by addressing all aspects of a product or service as perceived by users.
— Wikipedia
Human–Computer Interaction - Human–computer interaction (HCI) researches the design and use of computer technology, focusing particularly on the interfaces between people (users) and computers.
Researchers in the field of HCI both observe the ways in which humans interact with computers and design technologies that lets humans interact with computers in novel ways.
— Wikipedia
Minimally I'd suggest reading the following canonical texts on the matter so one can support and potential build usable user interfaces.
About Face: The Essentials of Interaction Design [read][$]
Design for Hackers: Reverse Engineering Beauty [read][$]
Design for Non-Designers [watch]
Designing Interfaces [read][$]
Designing Web Interfaces: Principles and Patterns for Rich Interactions [read][$]
Don't Make Me Think, Revisited: A Common Sense Approach to Web Usability [read][$]
3.8 - Learn HTML & CSS
HTML - HyperText Markup Language, commonly referred to as HTML, is the standard markup language used to create web pages. Web browsers can read HTML files and render them into visible or audible web pages. HTML describes the structure of a website semantically along with cues for presentation, making it a markup language, rather than a programming language.
— Wikipedia
CSS - Cascading Style Sheets (CSS) is a style sheet language used for describing the look and formatting of a document written in a markup language. Although most often used to change the style of web pages and user interfaces written in HTML and XHTML, the language can be applied to any kind of XML document, including plain XML, SVG and XUL. Along with HTML and JavaScript, CSS is a cornerstone technology used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.
— Wikipedia
Liken to constructing a house, one might consider HTML the framing and CSS to be the painting & decorating.
General Learning:
Absolute Centering in CSS [read]
CSS Positioning [watch][$]
Introduction to Web Development (v2) [watch][$]Front End Web Development: Get Started [watch][$]
Front-End Web Development Quick Start With HTML5, CSS, and JavaScript [watch][$]
HTML and CSS: Design and Build Websites [read][$]
HTML Document Flow [watch][$]
HTML Mastery: Semantics, Standards, and Styling [read][$]
Interneting is Hard [read]
Intro to HTML/CSS: Making webpages [watch]
Learn to Code HTML & CSS [read]
Learn CSS Layout [read]
MarkSheet [read]
MDN: HTML [read]
MDN: CSS [read]
Semantic HTML: How to Structure Web Pages [watch]
Solid HTML Form Structure [watch]
Understanding the CSS Box Model [watch]
Resilient Web Design [read]
Mastering CSS:
A Complete Guide to Flexbox [read]
CSS Grids and Flexbox for Responsive Web Design [watch][$]
CSS Diner [interact]
CSS Selectors from CSS4 till CSS1 [read]
CSS Secrets: Better Solutions to Everyday Web Design Problems [read][$]
CSS3 [read]CSS In-Depth, v2 [watch][$]
What the Flexbox?! A Simple, Free 20 Video Course That Will Help You
Master CSS
Flexbox [watch]
30 Seconds of CSS - A curated collection of useful CSS snippets you can understand in 30 seconds or less. [read]
References/Docs:

CSS Triggers...a Game of Layout, Paint, and Composite
cssreference.io
cssvalues.com
Default CSS for Chrome Browser
Head - A list of everything that could go in the of your document
HTML Attribute Reference
MDN CSS Reference
MDN HTML Element Reference
Glossary/Vocabulary:
CSS Glossary - Programming Reference for CSS Covering Comments, Properties, and Selectors
CSS Vocabulary
HTML Glossary Programming Reference for HTML elements
Standards/Specifications:
All W3C CSS Specifications
All W3C HTML Spec
Cascading Style Sheets Level 2 Revision 2 (CSS 2.2) SpecificationCSS Indexes - A listing of every term defined by CSS specs
The Elements of HTML from the Living Standard Global Attributes
The HTML Syntax from the Living Standard HTML 5.2 from W3C
Selectors Level 3
Architecting CSS:
Atomic Design [read]
BEM
ITCSS
OOCSS [read]
SMACSS [read][$]
Scalable Modular Architecture for CSS (SMACSS) [watch][$]
SUIT CSS
rscss
Authoring/Architecting Conventions:
CSS code guide [read]
css-architecture
cssguidelin.es [read]
Idiomatic CSS [read]
MaintainableCSS [read]
Standards for Developing Flexible, Durable, and Sustainable HTML and CSS [read]3.9 - Learn Search Engine Optimization
Search engine optimization (SEO) is the process of affecting the visibility of a website or a web page in a search engine's unpaid results — often referred to as "natural," "organic," or "earned" results. In general, the earlier (or higher ranked on the search results page), and more frequently a site appears in the search results list, the more visitors it will receive from the search engine's users. SEO may target different kinds of search, including image search, local search, video search, academic search, news search and industry-specific vertical search engines.
— Wikipedia
Image source: https://visual.ly/community/infographic/computers/how-does-seo-work
General Learning:
Google Search Engine Optimization Starter Guide [read]
Modern SEO [watch][$]
SEO Fundamentals From David Booth [watch][$]
SEO Fundamentals From Paul Wilson [watch][$]
SEO Tutorial For Beginners in 2016 [read]
SEO for Web Designers [watch][$]
3.10 - Learn JavaScript
JavaScript is a high level, dynamic, untyped, and interpreted programming language. It has been standardized in the ECMAScript language specification. Alongside HTML and CSS, it is one of the three essential technologies of World Wide Web content production; the majority of websites employ it and it is supported by all modern web browsers without plug-ins. JavaScript is prototype-based with first-class functions, making it a multi-paradigm language, supporting object-oriented, imperative, and functional programming styles. It has an API for working with text, arrays, dates and regular expressions, but does not include any I/O, such as networking, storage or graphics facilities, relying for these upon the host environment in which it is embedded.
— Wikipedia
Getting Started:
MDN: JavaScript [read]
javascript.info
JavaScript Enlightenment [read]
Eloquent JavaScript [read]
General Learning:
Speaking JavaScript [read]
JavaScript for impatient programmers [read]You Don't Know JS: Up & Going [read]
You Don't Know JS: Types & Grammar [read]
You Don't Know JS: Scope & Closures [read]
You Don't Know JS: this & Object Prototypes [read]
Modern JavaScript Cheatsheet - Cheatsheet for the JavaScript
knowledge you will frequently encounter in modern projects. [read]
JavaScript: The Hard Parts [watch][$]
Deep Foundations of JavaScript (v3) [watch][$]
Mastering:
Setting up ES6 [read]
ES6 FOR EVERYONE! [watch][$]
Exploring ES6 [read]
You Don't Know JS: ES6 & Beyond [read]
Understanding ECMAScript 6: The Definitive Guide for JavaScript Developers [read][$]
JavaScript: The Recent Parts [watch][$]
Exploring ES2016 and ES2017 [read]
Exploring ES2018 and ES2019 [read]
JavaScript Regular Expression Enlightenment [read]
Using Regular Expressions [watch][$]
You Don't Know JS: Async & Performance [read]
JavaScript with Promises [read][$]
Test-Driven JavaScript Development [read][$]
JS MythBusters [read]
Robust JavaScript [read]JavaScript Algorithms and Data Structures [read]
33 Concepts Every JavaScript Developer Should Know [read]
doesitmutate.xyz [read]
Functional JavaScript:
Functional Programming Jargon
funfunfunction: Functional programming in JavaScript [watch]
Functional-Light-JS [read]
Functional Programming in JavaScript: How to improve your JavaScript programs using functional techniques [read]
Mostly adequate guide to FP (in javascript) [read]
Professor Frisby Introduces Composable Functional JavaScript [watch]
JavaScript Allongé [read][$]
Functional-Lite JavaScript (v2) [watch][$]
Hardcore Functional Programming in JavaScript [watch][$]
References/Docs:
MDN JavaScript Reference
MSDN JavaScript Reference
Glossary/Encyclopedia/Jargon:
The JavaScript Encyclopedia
JavaScript Glossary
Simplified JavaScript Jargon
Standards/Specifications:How to Read the ECMAScript Specification
ECMAScript® 2015 Language Specification
ECMAScript® 2016 Language Specification
ECMAScript® 2017 Language Specification
ECMAScript® 2018 Language Specification
ECMAScript® 2019 Language Specification
Status, Process, and Documents for ECMA262
Style:
Airbnb JavaScript Style Guide
JavaScript Standard Style
JavaScript Semi-Standard Style
Deprecated JS Learning Resources:
Crockford on JavaScript - Volume 1: The Early Years [watch]
Crockford on JavaScript - Chapter 2: And Then There Was JavaScript [watch]
Crockford on JavaScript - Act III: Function the Ultimate [watch]
Crockford on JavaScript - Episode IV: The Metamorphosis of Ajax [watch]
Crockford on JavaScript - Part 5: The End of All Things [watch]
Crockford on JavaScript - Scene 6: Loopage [watch]
JavaScript Patterns [read][$]
The Principles of Object-Oriented JavaScript [read][$]
JavaScript Modules [read]
Functional JavaScript: Introducing Functional Programming with Underscore.js [read][$]
The Good Parts of JavaScript and the Web [watch][$]
High Performance JavaScript (Build Faster Web Application Interfaces) [read][$]
JS Explorers/Visualizers:
JavaScript Array Explorer
JavaScript Object Explorer
JavaScript Visualizer
3.11 - Learn DOM, BOM, CSSOM & jQuery
DOM - The Document Object Model (DOM) is a cross-platform and language-independent convention for representing and interacting with objects in HTML, XHTML, and XML documents. The nodes of every document are organized in a tree structure, called the DOM tree.
Objects in the DOM tree may be addressed and manipulated by using methods on the objects. The public interface of a DOM is specified in its application programming interface (API).
— Wikipedia
BOM - The Browser Object Model (BOM) is a browser-specific convention referring to all the objects exposed by the web browser.
Unlike the Document Object Model, there is no standard for implementation and no strict definition, so browser vendors are free to implement the BOM in any way they wish.
— WikipediajQuery - jQuery is a cross-platform JavaScript library designed to simplify the client-side scripting of HTML. jQuery is the most popular JavaScript library in use today, with installation on 65% of the top 10 million highest-trafficked sites on the Web. jQuery is free, open-source software licensed under the MIT License.
— Wikipedia
The ideal path, but certainly the most difficult, would be to first learn JavaScript, then the DOM, then jQuery. However, do what makes sense to your brain. Most front-end developers learn about JavaScript and then DOM by way of first learning jQuery. Whatever path you take, just make sure JavaScript, the DOM, and jQuery don't become a black box.
General Learning:
The Document Object Model [read]

HTML/JS: Making Webpages Interactive [watch]
HTML/JS: Making Webpages Interactive with jQuery [watch]
jQuery Enlightenment [read]
What is the DOM? [read]
Mastering:
AdvancED DOM Scripting: Dynamic Web Design Techniques [read][$]
Advanced JS Fundamentals to jQuery & Pure DOM Scripting [watch][$]
Douglas Crockford: An Inconvenient API - The Theory of the DOM [watch]
DOM Enlightenment [read][$] or read online for free
Fixing Common jQuery Bugs [watch][$]
jQuery-Free JavaScript [watch][$]
jQuery Tips and Tricks [watch][$]
References/Docs:
jQuery Docs
Events
DOM Browser Support
DOM Events Browser Support
HTML Interfaces Browser Support
MDN Document Object Model (DOM)
MDN Browser Object Model
MDN Document Object Model
MDN Event reference
MSDN Document Object Model (DOM)
CSS Object Model (CSSOM)
Standards/Specifications:
Document Object Model (DOM) Level 3 Events Specification
Document Object Model (DOM) Technical Reports
DOM Living Standard
W3C DOM4
3.12 - Learn Web Animation
General Learning:
SVG Essentials and Animation, v2 [$][watch]
Adventures in Web Animations [$][watch]
Animating With Snap.svg [$][watch]
Animation in CSS3 and HTML5 [$][watch]
Create Animations in CSS [read & watch]
CSS Animation in the Real World [$][watch]
Foundation HTML5 Animation with JavaScript [$][read]
Learn to Create Animations in JavaScript [read & watch]
Motion Design with CSS [$][watch]
State of the Animation 2015 [watch]
Web Animation using JavaScript: Develop & Design (Develop and Design) [$][read]
Standards/Specifications:
Web Animations
3.13 - Learn Web Fonts, Icons, & Images
Web typography refers to the use of fonts on the World Wide Web. When HTML was first created, font faces and styles were controlled exclusively by the settings of each Web browser. There was no mechanism for individual Web pages to control font display untilNetscape introduced the <font> tag in 1995, which was then standardized in the HTML 3.2 specification. However, the font specified by the tag had to be installed on the user's computer or a fallback font, such as a browser's default sans-serif or monospace font, would be used. The first Cascading Style Sheets specification was published in 1996 and provided the same capabilities.
The CSS2 specification was released in 1998 and attempted to improve the font selection process by adding font matching, synthesis and download. These techniques did not gain much use, and were removed in the CSS2.1 specification. However, Internet Explorer added support for the font downloading feature in version 4.0, released in 1997. Font downloading was later included in the CSS3 fonts module, and has since been implemented in Safari 3.1, Opera 10 and Mozilla Firefox 3.5.
This has subsequently increased interest in Web typography, as well as the usage of font downloading.
— Wikipedia
Fonts:
A Comprehensive Guide to Font Loading Strategies [read]
Beautiful Web Type a Showcase of the Best Typefaces from the Google Web Fonts Directory [read]
Quick Guide to Webfonts via @font-face [read]
MDN: Web fonts [read]
Responsive Web Typography, v2 [watch][$]
Typography for the Web [watch][$]
Icons:[read] [watch]
Images:
MDN: Images in HTML [read]
MDN: Responsive images [read]
SVG ON THE WEB - A Practical Guide [read]
3.14 - Learn Accessibility
Accessibility refers to the design of products, devices, services, or environments for people with disabilities. The concept of accessible design ensures both “direct access” (i.e., unassisted) and "indirect access" meaning compatibility with a person's assistive technology (for example, computer screen readers).
Accessibility can be viewed as the "ability to access" and benefit from some system or entity. The concept focuses on enabling access for people with disabilities, or special needs, or enabling access through the use of assistive technology; however, research and development in accessibility brings benefits to everyone.

Accessibility is not to be confused with usability, which is the extent to which a product (such as a device, service, or environment) can be used by specified users to achieve specified goals with effectiveness, efficiency and satisfaction in a specified context of use.Accessibility is strongly related to universal design which is the process of creating products that are usable by people with the widest possible range of abilities, operating within the widest possible range of situations. This is about making things accessible to all people (whether they have a disability or not).
— Wikipedia
General Learning:
9 tips to get bare minimum of web accessibility
Foundations of UX: Accessibility [watch][$]
How HTML elements are supported by screen readers [read]
Introduction to Web Accessibility - WAI [read]
Universal Design for Web Applications: Web Applications That Reach Everyone [read][$]
Web Accessibility: Getting Started [watch][$]
A Web for Everyone [read][$]
Web Accessibility [watch][$]
A11ycasts [watch]
Accessibility by Google - Udacity course [watch]
Standards/Specifications:
Accessible Rich Internet Applications (WAI-ARIA) Current Status
Web Accessibility Initiative (WAI)
Web Content Accessibility Guidelines (WCAG) Current Status
3.15 - Learn Web/Browser APIs
Image source: http://www.evolutionoftheweb.com/
The BOM (Browser Object Model) and the DOM (Document Object Model) are not the only browser APIs that are made available on the web platform inside of browsers. Everything that is not specifically the
DOM or BOM, but an interface for programming the browser could be considered a web or browser API (tragically in the past some of these APIs have been called HTML5 APIs which confuses their own specifics/standardize with the actual HTML5 specification specifying the HTML5 markup language). Note that web or browser APIs do include device APIs (e.g., Navigator.getBattery()) that are available through the browser on tablet andphones devices.
You should be aware of and learn, where appropriate, web/browser APIs. A good tool to use to familiarize oneself with all of these APIs would be to investigate the HTML5test.com results for the 5 most current browsers.
MDN has a great deal of information about web/browser APIs.
MDN Web API Reference
MDN Web APIs Interface Reference - All Interfaces, Arranged Alphabetically
MDN WebAPI - Lists Device Access APIs and Other APIs Useful for Applications
Keep in mind that not every API is specified by the W3C or WHATWG.
In addition to MDN, you might find the following resources helpful for learning about all the web/browser API's:
The HTML 5 JavaScript API Index
HTML5 Overview
platform.html5.org
3.16 - Learn JSON (JavaScript Object Notation)
JSON, (canonically pronounced sometimes JavaScript Object Notation), is an open standard format that uses human-readable text to transmit data objects consisting of attribute–value pairs. It is the primary dataformat used for asynchronous browser/server communication (A JA J), largely replacing XML (used by A JAX).
Although originally derived from the JavaScript scripting language, JSON is a language-independent data format. Code for parsing and generating JSON data is readily available in many programming languages.
The JSON format was originally specified by Douglas Crockford. It is currently described by two competing standards, RFC 7159 and ECMA-404. The ECMA standard is minimal, describing only the allowed grammar syntax, whereas the RFC also provides some semantic and security considerations. The official Internet media type for JSON is application/json. The JSON filename extension is .json.
— Wikipedia
General Learning:
Introduction to JavaScript Object Notation: A To-the-Point Guide to JSON [read][$]
json.com [read]
What is JSON [watch]
References/Docs:
json.org [read]
Standards/Specifications:
ECMA-404 The JSON Data Interchange Format
RFC 7159 The JavaScript Object Notation (JSON) Data Interchange FormatSTD 90 - RFC 8259 - The JavaScript Object Notation (JSON) Data Interchange
Format, DECEMBER 2017
Architecting:
JSON API
3.17 - Learn JS Templates
A JavaScript template is typically used, but not always with a MV* solution to separate parts of the view (i.e., the UI) from the logic and model (i.e., the data or JSON).
ES6 Template Literals, the Handlebars killer? [read]
Getting Started with nunjucks [read]
[read][$]
Lodash Templates [docs]
Note that JavaScript 2015 (aka ES6) added a native templating mechanism called "Templates strings". Additionally, templating as of late has been replaced by things like JSX, a template element, or HTML strings.
If I was not using React & JSX I'd first reach for JavaScript "Templates
strings" and when that was lacking move to nunjucks.

3.18 - Learn Static Site Generators
Static site generators, typically written using server side code (i.e., ruby, php, python, nodeJS, etc.), produce static HTML files from static text/data + templates that are intended to be sent from a server to the client statically without a dynamic nature.
General Learning:
JAMstack [read]
Static Site Generators [read]
Working with Static Sites - Bringing the Power of Simplicity to Modern Sites [read][$]
3.19 - Learn Computer Science via JS
Four Semesters of Computer Science in Six Hours [video][$]
Four Semesters of Computer Science in Six Hours: Part 2 [video][$]
Computer Science in JavaScript [read]
Collection of classic computer science paradigms, algorithms, and approaches written in JavaScript [read]
A Practical Guide to Algorithms with JavaScript [watch][$]
Introduction to Data Structures for Interviews [watch][$]
JavaScript Algorithms and Data Structures Masterclass [watch][$]
3.20 - Learn Front-End Application ArchitectureGeneral Learning:
Grab Front End Guide [read]
A set of best practices for JavaScript projects
Spellbook of Modern Web Dev
JavaScript Stack from Scratch
Deprecated Learning Materials:
JavaScript Application Design [read][$]
Build an App with React and Ampersand [watch]
Field Guide to Web Applications [read]
Frontend Guidelines Questionnaire [read]
Human JavaScript [read]
Nicholas Zakas: Scalable JavaScript Application Architecture [watch]
Organizing JavaScript Functionality [watch][$]
Patterns for Large-Scale JavaScript Application Architecture [read]
Terrific [read]
frontend case studies [read]
Not a lot of general content is being created on this topic as of late. Most of the content offered for learning how to build front-end/SPA/JavaScript applications presupposes you've decided up a tool like Angular, Ember, React, or Aurelia.
My advice, in 2019 learn React and Mobx and Apollo/graphql.
3.21 - Learn Data (i.e. JSON) API DesignAPI Design, v3 [watch][$]
Build APIs You Won't Hate [$][read]
JSON API [read]
3.22 - Learn React
Learning React:
Tutorial: Intro To React [read]
ReactJS For Stupid People [read]
The Beginner's Guide to ReactJS [watch]
Complete Intro to React v4 [watch][$]
React [read]
React Patterns Video Subscription [watch][$]
React Enlightenment [read]
REACT JS TUTORIAL #1 - Reactjs Javascript Introduction & Workspace Setup [watch]
Mastering React:
Build Your First Production Quality React App [watch][$]
Advanced React Component Patterns [watch][$]
Intermediate React [watch][$]
React Patterns [read]
8 Key React Component Decisions [read]
React - Basic Theoretical Concepts [read]
React + Mobx codebase containing real world examples (CRUD, auth, advanced patterns, etc) that adheres to the RealWorld spec and API. [code]
An Introduction to React Router v4 and its Philosophy Toward Routing [read]
Once you have a good handle on React move on to learning a more robust state management solution like MobX. If you are an experienced developer with Functional Programming knowledge look at Redux. If you need help understanding the role of state management beyond React's setState watch, "Advanced State Management in React (feat. Redux and MobX)".
3.23 - Learn Application State Management
State management in JavaScript [read]
Advanced State Management in React (feat. Redux and MobX) [watch][$]
React js tutorial - How Redux Works [watch]
MobX + React is AWESOME [watch]
3.24 - Learn Progressive Web App
Unlike traditional applications, progressive web apps are a hybrid of regular web pages (or websites) and a mobile application. This new“ application model attempts to combine features offered by most modern browsers with the benefits of mobile experience.
In 2015, designer Frances Berriman and Google Chrome engineer Alex Russell coined the term "Progressive Web Apps" to describe apps taking advantage of new features supported by modern browsers, including Service Workers and Web App Manifests, that let users upgrade web apps to be first-class applications in their native OS.
According to Google Developers, these characteristics are:
Progressive - Work for every user, regardless of browser choice because they’re built with progressive enhancement as a core tenet.
Responsive - Fit any form factor: desktop, mobile, tablet, or forms yet to emerge.

Connectivity independent - Service workers allow work offline, or on low quality networks.
App-like - Feel like an app to the user with app-style interactions and navigation.
Fresh - Always up-to-date thanks to the service worker update process.
Safe - Served via HTTPS to prevent snooping and ensure content hasn’t been tampered with.
Discoverable - Are identifiable as “applications”thanks to W3C manifests[6] and service worker registration scope allowing search engines to find them.
Re-engageable - Make re-engagement easy through features like push notifications.
Installable - Allow users to “keep” apps they find most useful on their home screen without the hassle of an app store.
Linkable - Easily shared via a URL and do not require complex installation.
— Wikipedia
A Beginnerʼs Guide To Progressive Web Apps [read]
Progressive Web Apps [read]
Getting Started with Progressive Web Apps [watch][$]
Building a Progressive Web App [watch][$]
Intro to Progressive Web Apps by Google [watch]
Native Apps are Doomed [read]
Why Native Apps Really are Doomed: Native Apps are Doomed pt 2 [read]
Your First Progressive Web App [read]
Progressive Web Applications and Offline [watch][$]
3.25 - Learn JS API Design
Designing Better JavaScript APIs [read]
Writing JavaScript APIs [read]
3.26 - Learn Browser Web Developer Tools
Web development tools allow web developers to test and debug their code. They are different from website builders and IDEs in that they do not assist in the direct creation of a webpage, rather they are tools used for testing the user facing interface of a website or web application.
Web development tools come as browser add-ons or built in features in web browsers. The most popular web browsers today like, Google Chrome, Firefox, Opera, Internet Explorer, and Safari have built in tools to help web developers, and many additional add-ons can be found in their respective plugin download centers.
Web development tools allow developers to work with a variety of web technologies, including HTML, CSS, the DOM, JavaScript, and other components that are handled by the web browser. Due to the increasing demand from web browsers to do more popular web browsers have included more features geared for developers.
— Wikipedia
While most browsers come equipped with web developer tools, the Chrome developer tools are currently the most talked about and widely used.
I'd suggest learning and using the Chrome web developer tools, simply because the best resources for learning web developer tools revolves around Chrome DevTools.
Learn Chrome Web Developer Tools:
Chrome Developer Tools [watch][$]
Explore and Master Chrome DevTools [watch]
Mastering Chrome Developer Tools v2 [watch][$]
Using The Chrome Developer Tools [watch][$]
Learning Chrome Web Developer Tools [watch][$]
Chrome Web Developer Tools Docs:
Command Line API Reference
Keyboard & UI Shortcuts Reference
Per-Panel Documentation
Configure and Customize DevTools
3.27 - Learn the Command Line (aka CLI)
A command-line interface or command language interpreter (CLI), also known as command-line user interface, console user interface, andcharacter user interface (CUI), is a means of interacting with a computer program where the user (or client) issues commands to the program in the form of successive lines of text (command lines).
— Wikipedia
General Learning:
The Bash Guide [read]
Command Line Power User [watch]
Learn Enough Command Line to Be Dangerous [read] [free to $]
Mastering:
Advanced Command Line Techniques [watch][$]
Introduction to Bash, VIM & Regex [watch][$]
3.28 - Learn Node.js
Node.js is an open-source, cross-platform runtime environment for developing server-side web applications. Node.js applications are written in JavaScript and can be run within the Node.js runtime on OS X, Microsoft Windows, Linux, FreeBSD, NonStop, IBM AIX, IBM System z and IBM i. Its work is hosted and supported by the Node.js Foundation, a collaborative project at Linux Foundation.Node.js provides an event-driven architecture and a non-blocking I/O API designed to optimize an application's throughput and scalability for real-time web applications. It uses Google V8 JavaScript engine to execute code, and a large percentage of the basic modules are written in JavaScript. Node.js contains a built-in library to allow applications to act as a web server without software such as Apache HTTP Server, Nginx or IIS.
— Wikipedia
General Learning:
The Art of Node [read]
Introduction to Node.js [watch][$]
Introduction to Node.js from Evented Mind [watch]
io.js and Node.js Next: Getting Started [watch][$]
Learning Node: Moving to the Server-Side [read][$]
Learn You The Node.js [self-guided workshops]
Node.js Basics [watch][$]
Node.js in Practice [read][$]
Real-time Web with Node.js [watch]
API Design in Node.js, v3 [watch][$]
Learn Node [watch][$]
3.29 - Learn ModulesGeneral Learning:
JavaScript for impatient programmers - Modules [read]
ES6 Modules in Depth [read]
Exploring JS - Modules [read]
ES modules: A cartoon deep-dive [read]
References/Docs:
MDN - export
MDN - import
3.30 - Learn Module loaders/bundlers
Webpack:
Webpack [read]
Webpack 4 Fundamentals [watch][$]
Survivejs.com Webpack Book [read]
Rollup:
Rollup [read]
Microbundle
Parcel
Parcel [read]
3.31 - Learn Package Manager
A package manager or package management system is a collection of software tools that automates the process of installing, upgrading, configuring, and removing software packages for a computer's operating system in a consistent manner. It typically maintains a database of software dependencies and version information to prevent software mismatches and missing prerequisites.
— Wikipedia
General Learning:
An introduction to how JavaScript package managers work [read]
The Mystical & Magical SemVer Ranges Used By npm & Bower [read]
Package Managers: An Introductory Guide For The Uninitiated Front-End Developer [read]
npm docs
yarn docs
3.32 - Learn Version Control“
A component of software configuration management, version control, also known as revision control or source control, is the management of changes to documents, computer programs, large web sites, and other collections of information. Changes are usually identified by a number or letter code, termed the "revision number," "revision level," or simply "revision." For example, an initial set of files is "revision 1." When the first change is made, the resulting set is "revision 2," and so on. Each revision is associated with a timestamp and the person making the change. Revisions can be compared, restored, and with some types of files, merged.
— Wikipedia
The most common solution used for version control today is Git. Learn it!
General Learning:
Getting Git Right [read]
Git Fundamentals [watch][$]
learn Enough Git [read]
Ry's Git Tutorial [read]
Mastering:
Git In-depth [watch][$]
Advanced Git Tutorials [read]
Pro Git [read]
Learn Git Branching [interact]
References/Docs:https://git-scm.com/doc
git-cheatsheet
3.33 - Learn Build and Task Automation
Build automation is the process of automating the creation of a software build and the associated processes including: compiling computer source code into binary code, packaging binary code, and running automated tests.
— Wikipedia
General Learning:
Getting Started with Gulp [read][$]
Gulp Basics [watch][$]
JavaScript Build Automation With Gulp.js [watch][$]
References/Docs:
Gulp
Gulp is great. However, you might only need npm run. Before turning to additional complexity in your application stack ask yourself if npm run can do the job. If you need more, use Gulp.Read:
Give Grunt the Boot! A Guide to Using npm as a Build Tool
Using npm as a Build System for Your next Project
Using npm as a Task Runner [watch][$]
Why I Left Gulp and Grunt for npm Scripts
Why npm Scripts?

3.34 - Learn Site Performance Optimization
Web performance optimization, WPO, or website optimization is the field of knowledge about increasing the speed in which web pages are downloaded and displayed on the user's web browser. With the average internet speed increasing globally, it is fitting for website administrators and webmasters to consider the time it takes for websites to render for the visitor.
— Wikipedia
General Learning:
Browser Rendering Optimization [watch]
Even Faster Web Sites: Performance Best Practices for Web Developers [read][$]
High Performance Web Sites: Essential Knowledge for Front-End Engineers [read][$]
JavaScript Performance Rocks [read][$]
PageSpeed Insights Rules [read]
perf-tooling.today [read]
Performance Calendar [read]
perf.rocks [read]
Using WebPageTest [read][$]
Web Performance Daybook Volume 2 [read][$]
Website Performance [watch][$]
Web Performance with Webpack 4 [watch][$]
Website Performance Optimization [watch]
Front-End Performance Checklist 2019 [PDF, Apple Pages, MS Word] [read]
3.35 - Learn Testing
Unit Testing - In computer programming, unit testing is a software testing method by which individual units of source code, sets of one or more computer program modules together with associated control
data, usage procedures, and operating procedures, are tested to determine whether they are fit for use. Intuitively, one can view a unit as the smallest testable part of an application.
— Wikipedia
Functional Testing - Functional testing is a quality assurance (QA)
process and a type of black box testing that bases its test cases on the specifications of the software component under test. Functions are tested by feeding them input and examining the output, and internal program structure is rarely considered (not like in white-box testing).
Functional testing usually describes what the system does.
— Wikipedia
Integration Testing - Integration testing (sometimes called integration and testing, abbreviated I&T) is the phase in software testing in which individual software modules are combined and tested as a group. It occurs after unit testing and before validation testing. Integration testing takes as its input modules that have been unit tested, groups them in larger aggregates, applies tests defined in an integration test plan to those aggregates, and delivers as its output the integrated system ready for system testing.
— Wikipedia
General Learning:
JavaScript Testing Practices and Principles [watch][$]
Front-End First: Testing and Prototyping JavaScript Apps [watch][$]
Let's Code: Test-Driven JavaScript [watch][$]
JavaScript Testing [watch]
JavaScript Testing Recipes [read][$]
Testable JavaScript [read][$]
Test-Driving JavaScript Applications: Rapid, Confident, Maintainable Code[read][$]
Test-Driven JavaScript Development [read][$]
The Way of the Web Tester: A Beginner's Guide to Automating Tests [read][$]
Testing React Applications, v2 [watch][$]
Learn Javascript Unit Testing With Mocha, Chai and Sinon [watch][$]
3.36 - Learn Headless Browsers
A headless browser is a web browser without a graphical user interface.
Headless browsers provide automated control of a web page in an environment similar to popular web browsers, but are executed via a command line interface or using network communication. They are particularly useful for testing web pages as they are able to render and understand HTML the same way a browser would, including styling elements such as page layout, color, font selection and execution of JavaScript and A JAX which are usually not available when using other testing methods. Google stated in 2009 that using a headless browser could help their search engine index content from websites that use AJAX.
— Wikipedia
Getting Started with Headless Chrome [readme]PhantomJS is no longer maintained, Headless Chrome steps in.
3.37 - Learn Offline Development
Offline development (aka offline first) is an area of knowledge and discussion around development practices for devices that are not always connected to the Internet or a power source.
General Learning:
Creating HTML5 Offline Web Applications [read]
Everything You Need to Know to Create Offline-First Web Apps [read]
Offline First [read]
offlinefirst.org [read]
The Offline Cookbook [read]
Offline Quickstart[read]
3.38 - Learn Web/Browser/App Security
Browser Security Handbook [read]
Frontend Security [watch]
Hacksplaining [read]
HTML5 Security Cheatsheet [read]
HTTP Security Best Practice [read]
Identity and Data Security for Web Development: Best Practices read
Security for Web Developers: Using JavaScript, HTML, and CSS [read][$]
The Basics of Web Application Security [read]
The Internet: Encryption & Public Keys [watch]
The Internet: Cybersecurity & Crime [watch]
The Tangled Web: A Guide to Securing Modern Web Applications [read][$]
Web Security Basics [read]
Web security [read]
Web Security [watch][$]
Full Stack for Front End Engineers [watch][$]
3.39 - Learn Multi-Device Development
Image source: http://bradfrost.com/blog/post/this-is-the-web/
A website or web application can run on a wide range of computers, laptops, tablets and phones, as well as a handful of new devices (watches, thermostats, fridges, etc.). How you determine what devices you'll support and how you will develop tosupport those devices is called, "multi-device development strategy". Below, I list the most common multi-device development strategies.
Build a responsive (RWD) web site/app for all devices.
Build an adaptive/progressively enhanced web site/app for all devices.
Build a website, web app, native app, or hybrid-native app for each individual device or a grouping of devices.
Attempt to retrofit something you have already built using bits and parts from strategies 1, 2 or 3.
General Learning:
A book Apart Pack - Responsive Web Design [read][$]
A Book Apart Pack - Design For Any Device [read][$]
Adaptive Web Design [read][$]
Designing with Progressive Enhancement [read][$]
Mobile Web Development [watch]
CSS Grids and Flexbox for Responsive Web Design [watch][$]
Responsive HTML Email Design [watch][$]
Responsive Images [watch]
Responsive Web Typography, v2 [watch][$]
Responsive Web Design Fundamentals [watch]
