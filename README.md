# 说明

这是我的编程语言学习笔记。如果能对你有所帮助，不胜荣幸。

目录（其它文件）：

- [F#学习笔记](./magic-fsharp.md)
- [Golang学习笔记](./golang-learning-notes.md)
- [Python学习笔记](./python-learning-notes.md)
- [C语言学习笔记](./c-learning-notes.md)
- [Elixir语言学习笔记](./elixir-learning-notes.md)
- [系统设计学习笔记](./system-design-reference.md)
- [常见的网络攻击手段和防御方法](./website-attack-and-defense.md)
- [技术大会介绍和资料](./tech-conference.md)
- [技术论文](./papers.md)

-------------------------------------------------------------------------------

# Books that I Have Read

## Common

- [Head First Object-Oriented Analysis and Design](https://book.douban.com/subject/1761742/)
- [Head First Design Patterns](https://book.douban.com/subject/1400656/)
- [重构 - Martin Fowler](https://book.douban.com/subject/4262627/)

## .NET Framework

- [CLR via C#](http://book.douban.com/subject/4924165/)
- [微软应用架构指南](https://book.douban.com/subject/5362857/)
- [Threading in C#](http://www.albahari.com/threading/)
- [.NET设计规范](https://book.douban.com/subject/4231292/)

## Golang

- [Go语言编程](https://book.douban.com/subject/11577300/)
- [An Introduction to Programming in Go](https://book.douban.com/subject/19897704/)

-------------------------------------------------------------------------------

# Guide

## Coding Style Guide

- [NET设计规范：约定、惯用法与模式](http://book.douban.com/subject/4231292/)
- [C# 3.0, C# 4.0 and C# 5.0 Coding Guidelines](http://csharpguidelines.codeplex.com/)
- [Google Style Guide](https://github.com/google/styleguide):  Style guides for Google-originated open-source projects
- [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
    - [JSCS — JavaScript Code Style](http://jscs.info/): JSCS is a code style linter/formatter for programmatically enforcing your style guide. You can configure JSCS for your project/company using over 150 validation rules, including presets from popular style guides like jQuery, Airbnb, Google, and more.

## Data Schema Design Guide

- [Bad Data Guide](https://github.com/Quartz/bad-data-guide): An exhaustive reference to problems seen in real-world data along with suggestions on how to resolve them.

## Web Development Guide

- [You-Dont-Know-JS](https://github.com/getify/You-Dont-Know-JS): This is a series of books diving deep into the core mechanisms of the JavaScript language.
- [Google Developers - Web Fundamentals](https://developers.google.com/web/fundamentals/): WebFundamentals is a comprehensive resource for web development best practices, designed to help you add the right features and experiences to your web project. If you’re new to web development or just looking to make your project better, we’ve got you covered.
- [You Don't Need jQuery](https://github.com/oneuijs/You-Dont-Need-jQuery): Examples of how to do query, style, dom, ajax, event etc like jQuery with plain javascript. This project summarizes most of the jQuery method alternatives in native implementation, with IE 10+ support.
- [Microsoft + Node.js Guidelines](https://github.com/Microsoft/nodejs-guidelines): Tips, tricks, and resources for working with Node.js, and the start of an ongoing conversation on how we can improve the Node.js experience on Microsoft platforms.
- [Learn javascript in one picture](https://github.com/coodict/javascript-in-one-pic)
- [Mars - mobile needs a hero](https://github.com/AlloyTeam/Mars): 面向亿万用户级的移动端Web解决方案
- [Frontend Development Bookmarks](https://github.com/dypsilon/frontend-dev-bookmarks): A huge list of frontend development resources I collected over time. Sorted from general knowledge at the top to concrete problems at the bottom.
- [The Elements of HTML](http://w3c.github.io/elements-of-html/)
- [A JavaScript Quality Guide](https://github.com/bevacqua/js)
- [Front-end-Developer-Interview-Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions): A list of helpful front-end related questions you can use to interview potential candidates, test yourself or completely ignore.

## Design Guide

- [Google Material Design](https://www.google.com/design/spec/material-design/introduction.html)

## DevOps

- [Logging best practices](http://dev.splunk.com/view/logging-best-practices/SP-CAAADP6)

-------------------------------------------------------------------------------

# Foundation, Organization, Specification

## Organization

Web:

- [MDN - Mozilla Developer Network](https://developer.mozilla.org/en-US/)
- [China W3C](http://www.chinaw3c.org)
- [Web Platform Docs](https://docs.webplatform.org/wiki/Main_Page)

.NET:

- [.NET Foundation](http://www.dotnetfoundation.org)
- [patterns & practices](https://msdn.microsoft.com/en-us/library/ff921345.aspx)
- [ServiceStack](https://servicestack.net/)
- [StackExchange](https://github.com/StackExchange)
- [Castle Projects](http://www.castleproject.org)
- [Mono Projects](https://github.com/mono)

## Specification

Web：

- HTML
    - [HTML - MDN](https://developer.mozilla.org/en-US/docs/Web/HTML)
    - [HTML5 - MDN](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
    - [HTML - WebPlantformDocs](https://docs.webplatform.org/wiki/html)
- CSS
    - [CSS - MDN](https://developer.mozilla.org/en-US/docs/Web/CSS)
    - [CSS3 - MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS3)
    - [CSS - WebPlantformDocs](https://docs.webplatform.org/wiki/css)
- JavaScript
    - [JavaScript - MDN](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript)
    - [ECMAScript Specification List](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Language_Resources)
    - [ECMAScript 6 入门](http://es6.ruanyifeng.com)
- DOM
    - [DOM - MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model)
- SVG
    - [SVG - MDN](https://developer.mozilla.org/en-US/docs/Web/SVG)
- WebGL
    - [WebGL - MDN](https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API)

通信协议：

- HTTP
    - [HTTP/2 Protocol](http://http2.github.io/): HTTP/2 is a replacement for how HTTP is expressed “on the wire.” It is not a ground-up rewrite of the protocol; HTTP methods, status codes and semantics are the same, and it should be possible to use the same APIs as HTTP/1.x (possibly with some small additions) to represent the protocol.
    - [HTTP/2 explained](http://http2-explained.readthedocs.org/en/latest/index.html): http2 explained describes the protocol HTTP/2 at a technical and protocol level. Background, the protocol, the implementations and the future. Written by Daniel Stenberg.
    - [HTTP 1.1 Protocol](http://www.w3.org/Protocols/): Hypertext Transfer Protocol 1.1 Specification
- WebSocket
    - [MDN - WebSockets](https://developer.mozilla.org/zh-CN/docs/WebSockets)
    - [HTML Living Standard - WebSocket](https://html.spec.whatwg.org/multipage/comms.html#network): this specification introduces the WebSocket interface
    - [RFC 6455 - The WebSocket Protocol](http://tools.ietf.org/html/rfc6455): The WebSocket Protocol
- Web Application Messaging Protocol
    - [WAMP - The Web Application Messaging Protocol](http://wamp-proto.org): WAMP is an open standard WebSocket subprotocol that provides two application messaging patterns in one unified protocol:
- RESTful API
    - [Wikipedia - RESTful API](https://en.wikipedia.org/wiki/Representational_state_transfer)
    - [Richardson Maturity Model](http://martinfowler.com/articles/richardsonMaturityModel.html)
- JSON
    - [JSON](http://json.org): JSON (JavaScript Object Notation) is a lightweight data-interchange format. It is easy for humans to read and write. It is easy for machines to parse and generate. It is based on a subset of the JavaScript Programming Language, Standard ECMA-262 3rd Edition - December 1999.
    - [JSON API](http://jsonapi.org/): A SPECIFICATION FOR BUILDING APIS IN JSON.
    - [JSON Schema & JSON Hyper-Schema](http://json-schema.org): JSON Schema: describes your JSON data format; JSON Hyper-Schema: turns your JSON data into hyper-text.
- OWIN
    - [OWIN - Open Web Interface for .NET](http://owin.org/)
- OData
    - [OData](http://www.odata.org/): OData is an OASIS standard for creating and consuming RESTful APIs.
- IPFS - The InterPlanetary File System
    - [IPFS](http://ipfs.io): The InterPlanetary File System (IPFS) is a new hypermedia distribution protocol, addressed by content and identities. IPFS enables the creation of completely distributed applications. It aims to make the web faster, safer, and more open.

参考：

- IoT
    - [Internet of Things Protocols & Standards](http://postscapes.com/internet-of-things-protocols)
    - [Understanding The Protocols Behind The Internet Of Things](http://electronicdesign.com/iot/understanding-protocols-behind-internet-things)
- Bitcoin
    - [Bitcoin Network](https://en.wikipedia.org/wiki/Bitcoin_network)
    - [Bitcoin wiki](https://en.bitcoin.it/wiki/Main_Page)
    - [Bitcoin](https://bitcoin.org/en/): Bitcoin is an innovative payment network and a new kind of money.

-------------------------------------------------------------------------------

# Projects

- [Framework & Libs](./projects-part-1.md)
- [Distributed Architecture](./projects-part-2.md)
- [Data Storage and Analysis](./projects-part-3.md)
- [DevOps](./projects-part-4.md)

# Articles

- [.NET Language & CLR](./articles-part-1.md)
- [Distributed Architecture](./articles-part-2.md)
- [Data Storage and Analysis](./articles-part-3.md)
- [DevOps](./articles-part-4.md)

-------------------------------------------------------------------------------

# References

- [official home of .NET on GitHub](https://github.com/microsoft/dotnet): dotnet is the official home of .NET on GitHub. It's a great starting point to find many .NET OSS projects from Microsoft and the community, including many that are part of the .NET Foundation.
- [Patterns & Practices](https://msdn.microsoft.com/en-us/library/ff921345.aspx)
- [Awesome dotNET](https://github.com/quozd/awesome-dotnet)
- [Open Source Testing](http://www.opensourcetesting.org/)
- [NoSQL Database](http://nosql-database.org/)
- [amplab - UC BERKELEY](https://amplab.cs.berkeley.edu/)
- [A Complete List of .NET Open Source Developer Projects](http://scottge.net/2015/07/08/a-complete-list-of-net-open-source-developer-projects/)
- [Essential JavaScript website](https://github.com/ericelliott/essential-javascript-links)
