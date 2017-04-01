<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Projects about Normal Software Development](#projects-about-normal-software-development)
    - [Compiler & CLR Framework](#compiler-clr-framework)
    - [Assembly Manipulation](#assembly-manipulation)
    - [Web Server](#web-server)
    - [Web Frameworks/Application Frameworks](#web-frameworksapplication-frameworks)
    - [Template Engine](#template-engine)
    - [Web Servers & Hosts](#web-servers-hosts)
    - [WebSocket](#websocket)
    - [Network](#network)
    - [Authentication && Authorization](#authentication-authorization)
    - [Data Access](#data-access)
    - [ORM framework](#orm-framework)
    - [Serialization & Deserialization](#serialization-deserialization)
    - [Windows Services](#windows-services)
    - [State Machine](#state-machine)
    - [Profiler](#profiler)
    - [Interoperability](#interoperability)
    - [IoC](#ioc)
    - [Logging](#logging)
    - [Cryptography](#cryptography)
    - [Compression](#compression)
    - [Mail](#mail)
    - [CLI](#cli)
    - [Manipulate Documents](#manipulate-documents)
    - [Manipulate Texts](#manipulate-texts)
    - [Report](#report)
    - [Tools](#tools)
    - [Math](#math)
    - [Image Processing](#image-processing)
    - [Misc Libraries](#misc-libraries)

<!-- /TOC -->

# Projects about Normal Software Development

## Compiler & CLR Framework

- [.NET Framewrok](https://msdn.microsoft.com/en-us/vstudio/aa496123.aspx)
- [.NET Core](http://dotnet.github.io/core/): A general purpose managed framework
- [.NET: Mono](http://www.mono-project.com/): Cross platform, open source .NET framework
- [.NET: Roslyn](https://github.com/dotnet/roslyn): The .NET Compiler Platform ("Roslyn") provides open-source C# and Visual Basic compilers with rich code analysis APIs.

## Assembly Manipulation

- [Fody](https://github.com/Fody/Fody) - Extensible tool for weaving .net assemblies
- [Mono.Cecil](https://github.com/jbevain/cecil) - Cecil is a library to generate and inspect programs and libraries in the ECMA CIL form.

## Web Server

- [.NET: KestrelHttpServer](https://github.com/aspnet/KestrelHttpServer): A web server for ASP.NET 5 based on libuv.

## Web Frameworks/Application Frameworks

- ASP.NET MVC
    - [ASP.net MVC 6](https://github.com/aspnet/Mvc): Model view controller framework for building dynamic web sites with clean separation of concerns, including the merged MVC, Web API, and Web Pages, Razor.
    - [ASP.net MVC 5](http://aspnetwebstack.codeplex.com/): ASP.NET MVC gives you a powerful, patterns-based way to build dynamic websites that enables a clean separation of concerns and that gives you full control over markup for enjoyable, agile development. ASP.NET MVC includes many features that enable fast, TDD-friendly development for creating sophisticated applications that use the latest web standards.
    - [ASP.NET Boilerplate](https://github.com/aspnetboilerplate/aspnetboilerplate) - A starting point for new modern ASP.NET MVC web applications with best practices and most popular tools.
- [ASP.net Web API 2](http://www.asp.net/web-api): ASP.NET Web API is a framework that makes it easy to build HTTP services that reach a broad range of clients, including browsers and mobile devices. ASP.NET Web API is an ideal platform for building RESTful applications on the .NET Framework.
    - [WebAPI Contrib](https://github.com/WebApiContrib/WebAPIContrib) - Collection of open source projects to help improve your work with ASP.NET Web API
- [.NET: Orleans](https://github.com/dotnet/orleans): Orleans is a framework that provides a straightforward approach to building distributed high-scale computing applications, without the need to learn and apply complex concurrency or other scaling patterns.
- [.NET: ServiceStack](https://github.com/ServiceStack/ServiceStack): Simple, Fast, Versatile and full-featured Services Framework
- [.NET: NancyFx](http://nancyfx.org/): Lightweight, low-ceremony, framework for building HTTP based services on .Net and Mono
- [.NET: ReactJS.NET](http://reactjs.net/): ReactJS.NET makes it easier to use Facebook's React and JSX from C# and other .NET languages, focusing specifically on ASP.NET MVC (although it also works in other environments). It assumes you already have some basic knowledge about React. It is cross-platform and can run on Linux via Mono. Now with support for ASP.NET 5 Beta!
- [Java: Spring Framework](http://spring.io/projects): The Spring Framework provides a comprehensive programming and configuration model for modern Java-based enterprise applications - on any kind of deployment platform.
    - [jHipster](https://jhipster.github.io/): Open Source application generator for creating Spring Boot + AngularJS projects in seconds

## Template Engine

- [.NET: RazorEngine](https://github.com/Antaris/RazorEngine): Open source templating engine based on Microsoft's Razor parsing engine
- [.NET: Nustache](https://github.com/jdiamond/Nustache): Logic-less templates for .NET
- [.NET: dotliquid](http://dotliquidmarkup.org/): a templating system ported to the .net framework from Ruby’s Liquid Markup.
- [.NET: StringTemplate](http://www.stringtemplate.org/): StringTemplate is a java template engine (with ports for C#, JavaScript, Python) for generating source code, web pages, emails, or any other formatted text output. StringTemplate is particularly good at code generators, multiple site skins, and internationalization / localization. StringTemplate also powers ANTLR.

## Web Servers & Hosts

- [Nginx](http://wiki.nginx.org/Main): a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
    - [OpenResty](http://openresty.org/): OpenResty (aka. ngx_openresty) is a full-fledged web application server by bundling the standard Nginx core, lots of 3rd-party Nginx modules, as well as most of their external dependencies.
    - [Tengine](http://tengine.taobao.org/): Tengine是由淘宝网发起的Web服务器项目。它在Nginx的基础上，针对大访问量网站的需求，添加了很多高级功能和特性。Tengine的性能和稳定性已经在大型的网站如淘宝网，天猫商城等得到了很好的检验。它的最终目标是打造一个高效、稳定、安全、易用的Web平台。
    - [VeryNginx](https://github.com/alexazhou/VeryNginx): 功能强大并且拥有对人类友好界面的Nginx, 提供防火墙，自定义行为和统计功能
- [.NET: Katana](http://katanaproject.codeplex.com/): As Web application development takes its next evolutionary step into the world of cloud computing, project Katana provides the underlying set of components to ASP.NET applications, enabling them to be flexible, portable, lightweight, and provide better performance – put another way, project Katana cloud optimizes your
- [lightttpd](http://www.lighttpd.net/): Security, speed, compliance, and flexibility -- all of these describe lighttpd (pron. lighty) which is rapidly redefining efficiency of a webserver; as it is designed and optimized for high performance environments. With a small memory footprint compared to other web-servers, effective management of the cpu-load, and advanced feature set (FastCGI, SCGI, Auth, Output-Compression, URL-Rewriting and many more) lighttpd is the perfect solution for every server that is suffering load problems. And best of all it's Open Source licensed under the revised BSD license.

## Asynchronous Programming Framework

- [ReactiveX](http://reactivex.io/): An API for asynchronous programming with observable streams
  - Java: RxJava
  - JavaScript: RxJS
  - C#: Rx.NET
  - C#(Unity): UniRx
  - Scala: RxScala
  - Clojure: RxClojure
  - C++: RxCpp
  - Lua: RxLua
  - Ruby: Rx.rb
  - Python: RxPY
  - Go: RxGo
  - Groovy: RxGroovy
  - JRuby: RxJRuby
  - Kotlin: RxKotlin
  - Swift: RxSwift
  - PHP: RxPHP
  - Elixir: reaxive
  - Dart: RxDart

## WebSocket

- [.NET: SignalR](https://github.com/SignalR/SignalR): Library for ASP.NET developers that makes it incredibly simple to add real-time web functionality to your applications
- [.NET: Fleck](https://github.com/statianzo/Fleck) - Fleck is a WebSocket server implementation in C#. Branched from the Nugget project
- [.NET: Websocket-Sharp](https://github.com/sta/websocket-sharp) - A C# implementation of the WebSocket protocol client and server
- [.NET: WebSocket4NET](https://websocket4net.codeplex.com/) - WebSocket client for .NET 2.0+, Xamarin, Mono, Silverlight, Windows Phone, & WinRT
- [.NET: XSockets](https://xsockets.net/) - Provides a great set of tools for you to build real-time applications on the Microsoft.NET plattform and much more
- [.NET: WampSharp](https://github.com/Code-Sharp/WampSharp) - A C# implementation of [The Web Application Messaging Protocol](http://wamp-proto.org/) - a protocol that provides messaging patterns of Remote Procedure Calls and Publish/Subscribe over WebSockets.

## Network

- [.NET: Fracture](https://github.com/fractureio/fracture): A high-performance socket I/O message pipeline library.
- [.NET: SuperSocket](http://www.supersocket.net/): SuperSocket 是一个轻量级, 跨平台而且可扩展的 .Net/Mono Socket 服务器程序框架。你无须了解如何使用 Socket, 如何维护 Socket 连接和 Socket 如何工作，但是你却可以使用 SuperSocket 很容易的开发出一款 Socket 服务器端软件，例如游戏服务器，GPS 服务器, 工业控制服务和数据采集服务器等等。
- [.NET: RestSharper](http://restsharp.org/): Simple REST and HTTP API Client for .NET

## Authentication && Authorization

- [.NET: ASP.NET Identity](https://aspnetidentity.codeplex.com/) - New membership system for ASP.NET applications
- [.NET: DotNetOpenAuth](https://github.com/DotNetOpenAuth/DotNetOpenAuth) - A C# implementation of the OpenID, OAuth and InfoCard protocols
- [.NET: IdentityModel](https://github.com/IdentityModel) - Helper library for identity & access control in .NET 4.5 and MVC4/Web API.
- [.NET: IdentityServer](https://github.com/IdentityServer) - Extensible OAuth2 and OpenID Connect provider framework.
- [.NET: OAuth](https://github.com/danielcrenna/oauth) - A very lightweight library for generating OAuth 1.0a signatures written in C#

## Data Access

- [.NET: StackExchange.Redis](https://github.com/StackExchange/StackExchange.Redis): a high performance general purpose redis client for .NET languages (C# etc)
- [.NET: SolrNet](https://github.com/mausch/SolrNet): SolrNet is an Apache Solr client for .NET
- [.NET: EasyNetQ](https://github.com/EasyNetQ/EasyNetQ): An easynet to use .NET API for RabbitMQ, not offical rabbitmq .net client
- [.NET: DbUtility](https://github.com/Ivony/DbUtility):  a light database access tool

## ORM framework

- [.NET: Drapper](https://github.com/StackExchange/dapper-dot-net): a simple object mapper for .Net
- [.NET: Entity Framework](https://github.com/aspnet/EntityFramework): Microsoft's recommended data access technology for new applications in .NET.
- [.NET: MyBatis](https://mybatis.github.io/): MyBatis is a first class persistence framework with support for custom SQL, stored procedures and advanced mappings. MyBatis eliminates almost all of the JDBC code and manual setting of parameters and retrieval of results. MyBatis can use simple XML or Annotations for configuration and map primitives, Map interfaces and Java POJOs (Plain Old Java Objects) to database records.
- [.NET: ServiceStack.OrmLite](https://github.com/ServiceStack/ServiceStack.OrmLite): Fast, Simple, Typed ORM for .NET
- [.NET: nhibernate](http://nhibernate.info/): NHibernate is a mature, open source object-relational mapper for the .NET framework. It's actively developed, fully featured and used in thousands of successful projects.
- [.NET: fluent-nhibernate](https://github.com/jagregory/fluent-nhibernate): Fluent, XML-less, compile safe, automated, convention-based mappings for NHibernate. Get your fluent on.

## Serialization & Deserialization

- [Java: fastjson](https://github.com/alibaba/fastjson): A fast JSON parser/generator for Java
- [.NET: Jil](https://github.com/kevin-montrose/Jil): Fast .NET JSON (De)Serializer, Built On Sigil
- [.NET: ServiceStack.Text](https://github.com/ServiceStack/ServiceStack.Text): .NET's fastest JSON, JSV and CSV Text Serializers
- [.NET: Json.net](http://www.newtonsoft.com/json): Popular high-performance JSON framework for .NET
- [.NET: fastjson](https://fastjson.codeplex.com/): Smallest, fastest polymorphic JSON serializer

## Windows Services

- [.NET: Topshelf](http://topshelf-project.com/): Put Your Apps on the Topshelf

## State Machine

- [.NET: Stateless](https://github.com/nblumhardt/stateless) - Create state machines and lightweight state machine-based workflows directly in .NET code
- [.NET: Automatonymous](https://github.com/MassTransit/Automatonymous) - A state machine library for .Net - allows you to write fluent style state machines

## Profiler

- [.NET: MiniProfiler](http://miniprofiler.com/): A simple but effective mini-profiler for .NET and Ruby
- [.NET: Glimpse](http://getglimpse.com/): Providing real time diagnostics & insights to the fingertips of hundreds of thousands of developers daily
- [.NET: metrics-net](https://github.com/danielcrenna/metrics-net): Capturing CLR and application-level metrics. So you know what's going on.
- [.NET: Metrics.NET](https://github.com/etishor/Metrics.NET): The Metrics.NET library provides a way of instrumenting applications with custom metrics (timers, histograms, counters etc) that can be reported in various ways and can provide insights on what is happening inside a running application.

## IoC

- [.NET: Castle Windsor](https://github.com/castleproject/Windsor) - Castle Windsor is best of breed, mature Inversion of Control container available for .NET and Silverlight
- [.NET: Unity](https://unity.codeplex.com/) - Lightweight extensible dependency injection container with support for constructor, property, and method call injection
- [.NET: Autofac](https://github.com/autofac/Autofac) - An addictive .NET IoC container
- [.NET: Ninject](https://github.com/ninject/ninject) - The ninja of .net dependency injectors
- [.NET: StructureMap](https://structuremap.github.io/) - The original IoC/DI Container for .Net
- [.NET: Spring.Net](https://github.com/spring-projects/spring-net) - Spring.NET is an open source application framework that makes building  enterprise .NET applications easier
- [.NET: LightInject](https://github.com/seesharper/LightInject) - A ultra lightweight IoC container
- [.NET: TinyIoC](https://github.com/grumpydev/TinyIoC) - Single-file, easy and cross-platform IoC container

## Logging

- [.NET: Essential Diagnostics](http://essentialdiagnostics.codeplex.com/) - Extends the inbuilt features of System.Diagnostics namespace to provide flexible logging
- [.NET: NLog](https://github.com/nlog/NLog/) - NLog - Advanced .NET and Silverlight Logging
- [.NET: Logary](http://logary.github.io/) - Logary is a high performance, multi-target logging, metric, tracing and health-check library for mono and .Net. .Net's answer to DropWizard. Supports many targets, built for micro-services.
- [.NET: Log4Net](https://logging.apache.org/log4net/) - The Apache log4net library is a tool to help the programmer output log statements to a variety of output targets
- [.NET: Serilog](https://github.com/serilog/serilog) - A no-nonsense logging library for the NoSQL era. Combines the best of traditional and structured diagnostic logging in an easy-to-use package.
- [.NET: StackExchange.Exceptional](https://github.com/NickCraver/StackExchange.Exceptional) - Error handler used for the Stack Exchange network

## Cryptography

- [BouncyCastle](https://bouncycastle.org/) - Together with the .Net System.Security.Cryptography, the reference implementation for cryptographic algorithms on the CLR.
- [HashLib](http://hashlib.codeplex.com/) - HashLib is a collection of nearly all hash algorithms you've ever seen, it supports almost everything and is very easy to use
- [libsodium-net](https://github.com/adamcaudill/libsodium-net) - libsodium for .NET - A secure cryptographic library
- [StreamCryptor](https://github.com/bitbeans/StreamCryptor) - Stream encryption & decryption with libsodium and protobuf

## Compression

- [SharpCompress](https://github.com/adamhathcock/sharpcompress) - SharpCompress is a compression library for .NET/Mono/Silverlight/WP7 that can unrar, un7zip, unzip, untar unbzip2 and ungzip with forward-only reading and file random access APIs. Write support for zip/tar/bzip2/gzip are implemented
- [DotNetZip.Semverd](https://github.com/haf/DotNetZip.Semverd) - An open-source project that delivers a .NET library for handling ZIP files, and some associated tools. (fork of Unmaintained DotNetZip)
- [SharpZipLib](http://icsharpcode.github.io/SharpZipLib/) - a Zip, GZip, Tar and BZip2 library written entirely in C# for the .NET platform

## Mail

- [FluentEmail](https://github.com/lukencode/FluentEmail): A Fluent Wrapper for System.Net.Mail with razor templating support.
- [MailKit](https://github.com/jstedfast/MailKit): A complete cross-platform mail stack including IMAP, POP3, SMTP, authentication and more. Built on top of MimeKit.
- [MimeKit](https://github.com/jstedfast/MimeKit): A cross-platform .NET MIME creation and parser library with support for S/MIME, PGP, TNEF and Unix mbox spools.
- [MailSystem.NET](https://mailsystem.codeplex.com/): MailSystem is a suite of .NET components that provide users with an extensive set of email tools. MailSystem provides full support for SMTP, POP3, IMAP4, NNTP, MIME, S/MIME, OpenPGP, DNS, vCard, vCalendar, Anti-Spam (Bayesian , RBL, DomainKeys), Queueing, Mail Merge and WhoIs. If you wish to use this code in non GPLv3 software, you must acquire a commercial license. Please send your request to the coordinator of this project.

## CLI

- [Command Line Parser](https://github.com/gsscoder/commandline) - The Command Line Parser Library offers to CLR applications a clean and concise API for manipulating command line arguments and related tasks
- [Fluent Command Line Parser](https://github.com/fclp/fluent-command-line-parser) - A simple, strongly typed .NET C# command line parser library using a fluent easy to use interface
- [Power Args](https://github.com/adamabdelhamed/PowerArgs) - PowerArgs converts command line arguments into .NET objects that are easy to program against. It also provides a ton of optional capabilities such as argument validation, auto generated usage, tab completion, and plenty of extensibility

## Tools

- [CS-Script](http://www.csscript.net/index.html): CS-Script is a CLR (Common Language Runtime) based scripting system which uses ECMA-compliant C# as a programming language. CS-Script currently targets Microsoft implementation of CLR (.NET 2.0/3.0/3.5/4.0/4.5) with full support on Mono.
- [Scriptcs](http://scriptcs.net/): Unleash your C# from Visual Studio.
- [dotPeek](https://www.jetbrains.com/decompiler/): Free .NET Decompiler and Assembly Browser
- [FastFileFinder](https://github.com/Wintellect/FastFileFinder): Find files and directory names FAST!
- [Rant2](https://github.com/TheBerkin/Rant): Rant is a language for procedurally generating text, written in C#. It combines a markup language with functional and imperative programming concepts to deliver a powerful, but easy-to-use tool for adding rich variations to your text. The ultimate goal of Rant is to augment your creativity with the boundless potential of randomness, helping you consider your next great idea as not just a static concept, but a seed for countless possibilities.

## Math

- [Math.NET Numerics: numerical computing](http://numerics.mathdotnet.com/): Math.NET Numerics aims to provide methods and algorithms for numerical computations in science, engineering and every day use. Covered topics include special functions, linear algebra, probability models, random numbers, interpolation, integration, regression, optimization problems and more.
- [Math.NET Symbolics: computer algebra](http://symbolics.mathdotnet.com/): Math.NET Symbolics is a basic open source computer algebra library for .Net and Mono written in F#.
- [Math.NET Filtering: signal processing](http://filtering.mathdotnet.com/): Filtering aims to provide a toolkit for digital signal processing, offering an infrastructure for digital filter design, applying those filters to data streams using data converters, as well as digital signal generators.
- [Math.NET Spatial](http://spatial.mathdotnet.com/): Math.NET Spatial is aiming to become a geometry library for .Net and Mono.

## Image Processing

- [nQuant .net Color Quantizer](https://nquant.codeplex.com/): nQuant is a .net color quantizer producing high quality 256 color 8 bit PNG images using an algorithm optimized for the highest quality possible.
- [OpenCV](http://opencv.org/): OpenCV is released under a BSD license and hence it’s free for both academic and commercial use. It has C++, C, Python and Java interfaces and supports Windows, Linux, Mac OS, iOS and Android. OpenCV was designed for computational efficiency and with a strong focus on real-time applications. Written in optimized C/C++, the library can take advantage of multi-core processing. Enabled with OpenCL, it can take advantage of the hardware acceleration of the underlying heterogeneous compute platform. Adopted all around the world, OpenCV has more than 47 thousand people of user community and estimated number of downloads exceeding 9 million. Usage ranges from interactive art, to mines inspection, stitching maps on the web or through advanced robotics.
    - [Emgu CV](http://www.emgu.com/wiki/index.php/Emgu_CV): Emgu CV is a cross platform .Net wrapper to the OpenCV image processing library. Allowing OpenCV functions to be called from .NET compatible languages such as C#, VB, VC++, IronPython etc. The wrapper can be compiled by Visual Studio, Xamarin Studio and Unity, it can run on Windows, Linux, Mac OS X, iOS, Android and Windows Phone.
- [AForge.NET](http://www.aforgenet.com/): AForge.NET is a C# framework designed for developers and researchers in the fields of Computer Vision and Artificial Intelligence - image processing, neural networks, genetic algorithms, machine learning, robotics, etc.
- [ImageMagick](http://www.imagemagick.org): ImageMagick® is a software suite to create, edit, compose, or convert bitmap images. It can read and write images in a variety of formats (over 200) including PNG, JPEG, JPEG-2000, GIF, TIFF, DPX, EXR, WebP, Postscript, PDF, and SVG. Use ImageMagick to resize, flip, mirror, rotate, distort, shear and transform images, adjust image colors, apply various special effects, or draw text, lines, polygons, ellipses and Bézier curves.
- [GraphicsMagick](http://www.graphicsmagick.org): GraphicsMagick is the swiss army knife of image processing. Comprised of 267K physical lines (according to David A. Wheeler's SLOCCount) of source code in the base package (or 1,225K including 3rd party libraries) it provides a robust and efficient collection of tools and libraries which support reading, writing, and manipulating an image in over 88 major formats including important formats like DPX, GIF, JPEG, JPEG-2000, PNG, PDF, PNM, and TIFF.
- [ImageProcessor](http://imageprocessor.org/): ImageProcessor is a collection of lightweight libraries written in C# that allows you to manipulate images on-the-fly using .NET 4.5+
- [Hugin](http://sourceforge.net/projects/hugin): Panorama photo stitcher
- [Luminance HDR](http://sourceforge.net/projects/qtpfsgui): Complete solution for HDR photography
- [scikit-image](http://scikit-image.org/): scikit-image is a collection of algorithms for image processing. It is available free of charge and free of restriction.
- $[Pano2VR && Object2VR](http://ggnome.com/): software for interactive panoramas and object movies.

## Interoperability

- [CppSharp](https://github.com/mono/CppSharp) - Tools to surface C++ APIs to C#
- [Sharpen](https://github.com/mono/sharpen) - Sharpen is an Eclipse plugin created by db4o that allows you to convert your Java project into C#
- [CXXI](https://github.com/mono/cxxi) - C++ interop framework

## Misc Libraries

- [AutoMapper](http://automapper.org/): a simple little library built to solve a deceptively complex problem - getting rid of code that mapped one object to another.
- [UrlRewriter](https://github.com/sethyates/urlrewriter): UrlRewriter.NET is an open-source, light-weight, highly configurable URL rewriting component for ASP.NET 1.1 – 4.0.
- [Fast Reflection Library](http://fastreflectionlib.codeplex.com/): FastReflectionLib provide the same as part of the refection features like executing method dynamically but give simple and faster implementations. It can be use as the foundation of reflection-based scenarios such as ORM framework.
- [FluentValidation](https://github.com/JeremySkinner/FluentValidation): A small validation library for .NET that uses a fluent interface and lambda expressions for building validation rules. Written by Jeremy Skinner (http://www.jeremyskinner.co.uk) and licensed under Apache 2.
- [.NET Extensions Methods Library for C# and VB.NET (ASP.NET, MVC, SL, WPF, EF)](https://dnpextensions.codeplex.com/)
- [Html Agility Pack](https://htmlagilitypack.codeplex.com/): This is an agile HTML parser that builds a read/write DOM and supports plain XPATH or XSLT (you actually don't HAVE to understand XPATH nor XSLT to use it, don't worry...). It is a .NET code library that allows you to parse "out of the web" HTML files. The parser is very tolerant with "real world" malformed HTML. The object model is very similar to what proposes System.Xml, but for HTML documents (or streams).
- [Base Class Libraries](https://bcl.codeplex.com/): The Base Class Libraries site hosts samples, previews, and prototypes from the BCL team.
This is a site for the BCL Team to get features to customers to try out without requiring a Beta or CTP of the .NET Framework. Our goal is to put generally useful functionality here, and to get feedback on it and have the chance to iterate on the design.
- [CommonLibrary.NET](https://commonlibrarynet.codeplex.com/): A collection of very reusable code and components in C# 4.0 ranging from ActiveRecord, Csv, Command Line Parsing, Configuration, Validation, Logging, Collections, Authentication, and much more. This is ideal for C# developer looking for a Utility library, Java developers looking for a C# version of Java Commons.
- [Craig-s-Utility-Library](http://jacraig.github.io/Craig-s-Utility-Library/): With .Net we have a number of built in classes and functions to help make a programmer's life easier, but let's face facts, they didn't think of everything. Craig's Utility Library tries to fill in some of those gaps (or at least the ones that I've run into). It comes with a couple hundred extension methods, built in data types such as a BTree, priority queue, ring buffer, etc. And that's just the DataTypes namespace. When you add it all up, Craig's Utility Library is one of the largest set of utilities for .Net out there.
- [Wintellect's Power Collections for .NET](http://powercollections.codeplex.com/): Power Collections makes heavy use of .NET Generics. The goal of the project is to provide generic collection classes that are not available in the .NET framework. Some of the collections included are the Deque, MultiDictionary, Bag, OrderedBag, OrderedDictionary, Set, OrderedSet, and OrderedMultiDictionary.
- [Humanizer](https://github.com/MehdiK/Humanizer): Humanizer meets all your .NET needs for manipulating and displaying strings, enums, dates, times, timespans, numbers and quantities
- [Wintellect PowerThreading](https://github.com/Wintellect/PowerThreading): Jeffrey Richter's Power Threading Library
- [Sigil](https://github.com/kevin-montrose/Sigil): A fail-fast validating helper for .NET CIL generation
- [Shielded](https://github.com/jbakic/Shielded): A strict and mostly lock-free Software Transactional Memory (STM) for .NET
- [NodaTime](https://github.com/nodatime/nodatime): A better date and time API for .NET
- [Peasy.NET](https://github.com/peasy/Peasy.NET): An easy to use middle tier framework for .net
