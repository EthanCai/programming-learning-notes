<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Projects about .NET](#projects-about-net)
	- [Compiler](#compiler)
	- [Decompiler](#decompiler)
	- [REPL](#repl)
	- [Assembly Manipulation](#assembly-manipulation)
	- [Web Servers & Application Servers](#web-servers-application-servers)
	- [Application Frameworks](#application-frameworks)
	- [Template Engine](#template-engine)
	- [Asynchronous Programming Framework](#asynchronous-programming-framework)
	- [Web Socket](#web-socket)
	- [Network](#network)
	- [Thread & Coroutine](#thread-coroutine)
	- [IoC](#ioc)
	- [Logging](#logging)
	- [Cryptography](#cryptography)
	- [Compression](#compression)
	- [Profiler](#profiler)
	- [Data Access](#data-access)
	- [Serialization & Deserialization](#serialization-deserialization)
	- [Command Line](#command-line)
	- [Math](#math)
	- [Image Processing](#image-processing)
	- [Computer Vision](#computer-vision)
	- [Authentication & Authorization](#authentication-authorization)
	- [Mail](#mail)
	- [State Machine](#state-machine)
	- [.NET Interoperability](#net-interoperability)
	- [Windows Services](#windows-services)
	- [Misc Libraries](#misc-libraries)

<!-- /TOC -->

# Projects about .NET

## Compiler

- [.NET Core](http://dotnet.github.io/core/): A general purpose managed framework
- [.NET: Mono](http://www.mono-project.com/): Cross platform, open source .NET framework
- [.NET: Roslyn](https://github.com/dotnet/roslyn): The .NET Compiler Platform ("Roslyn") provides open-source C# and Visual Basic compilers with rich code analysis APIs.

## Decompiler

- [.NET: dotPeek](https://www.jetbrains.com/decompiler/): Free .NET Decompiler and Assembly Browser
- [.NET: ILSpy](https://github.com/icsharpcode/ILSpy): .NET Decompiler

## REPL

- [.NET Fiddle](https://dotnetfiddle.net/)
- [CS-Script](http://www.csscript.net/index.html): CS-Script is a CLR (Common Language Runtime) based scripting system which uses ECMA-compliant C# as a programming language. CS-Script currently targets Microsoft implementation of CLR (.NET 2.0/3.0/3.5/4.0/4.5) with full support on Mono. uses ECMA-compliant C# as a programming language. CS-Script currently targets Microsoft implementation of CLR (.NET 2.0/3.0/3.5/4.0/4.5) with full support on Mono.
- [Scriptcs](http://scriptcs.net/): Unleash your C# from Visual Studio.

## Assembly Manipulation

- [.NET: Fody](https://github.com/Fody/Fody) - Extensible tool for weaving .net assemblies
- [.NET: Mono.Cecil](https://github.com/jbevain/cecil) - Cecil is a library to generate and inspect programs and libraries in the ECMA CIL form.

## Web Servers & Application Servers

- [.NET: KestrelHttpServer](https://github.com/aspnet/KestrelHttpServer): A cross platform web server for ASP.NET Core.

## Application Frameworks

- [.NET: ASP.net Core MVC](https://github.com/aspnet/Mvc): ASP.NET Core MVC is a model view controller framework for building dynamic web sites with clean separation of concerns, including the merged MVC, Web API, and Web Pages w/ Razor.
	- [.NET: ASP.NET Boilerplate](https://github.com/aspnetboilerplate/aspnetboilerplate) - A starting point for new modern ASP.NET MVC web applications with best practices and most popular tools. applications with best practices and most popular tools.
	- [.NET: ASP.net Web API 2](http://www.asp.net/web-api): ASP.NET Web API is a framework that makes it easy to build HTTP services that reach a broad range of clients, including browsers and mobile devices. ASP.NET Web API is an ideal platform for building RESTful applications on the .NET Framework.
	    - [.NET: WebAPI Contrib](https://github.com/WebApiContrib/WebAPIContrib) - Collection of open source projects to help improve your work with ASP.NET Web API
- [.NET: Orleans](https://github.com/dotnet/orleans): Orleans is a framework that provides a straightforward approach to building distributed high-scale computing applications, without the need to learn and apply complex concurrency or other scaling patterns.
- [.NET: ServiceStack](https://github.com/ServiceStack/ServiceStack): Simple, Fast, Versatile and full-featured Services Framework
- [.NET: NancyFx](http://nancyfx.org/): Lightweight, low-ceremony, framework for building HTTP based services on .Net and Mono
- [.NET: Katana](http://katanaproject.codeplex.com/): As Web application development takes its next evolutionary step into the world of cloud computing, project Katana provides the underlying set of components to ASP.NET applications, enabling them to be flexible, portable, lightweight, and provide better performance – put another way, project Katana cloud optimizes your

## Template Engine

- [.NET: RazorEngine](https://github.com/Antaris/RazorEngine): Open source templating engine based on Microsoft's Razor parsing engine
- [.NET: Nustache](https://github.com/jdiamond/Nustache): Logic-less templates for .NET
- [.NET: dotliquid](http://dotliquidmarkup.org/): a templating system ported to the .net framework from Ruby’s Liquid Markup.
- [.NET: StringTemplate](http://www.stringtemplate.org/): StringTemplate is a java template engine (with ports for C#, JavaScript, Python) for generating source code, web pages, emails, or any other formatted text output. StringTemplate is particularly good at code generators, multiple site skins, and internationalization / localization. StringTemplate also powers ANTLR.

## Asynchronous Programming Framework

- [ReactiveX](http://reactivex.io/): An API for asynchronous programming with observable streams
  - [C#: Rx.NET](https://github.com/Reactive-Extensions/Rx.NET)

## Web Socket

- [.NET: SignalR](https://github.com/SignalR/SignalR): Library for ASP.NET developers that makes it incredibly simple to add real-time web functionality to your applications
- [.NET: Fleck](https://github.com/statianzo/Fleck) - Fleck is a WebSocket server implementation in C#. Branched from the Nugget project
- [.NET: Websocket-Sharp](https://github.com/sta/websocket-sharp) - A C# implementation of the WebSocket protocol client and server
- [.NET: WebSocket4NET](https://websocket4net.codeplex.com/) - WebSocket client for .NET 2.0+, Xamarin, Mono, Silverlight, Windows Phone, & WinRT
- [.NET: XSockets](https://xsockets.net/) - Provides a great set of tools for you to build real-time applications on the Microsoft.NET plattform and much more
- [.NET: WampSharp](https://github.com/Code-Sharp/WampSharp) - A C# implementation of [The Web Application Messaging Protocol](http://wamp-proto.org/) - a protocol that provides messaging patterns of Remote Procedure Calls and Publish/Subscribe over WebSockets.

## Network

- [.NET: RestSharper](http://restsharp.org/): Simple REST and HTTP API Client for .NET
- [.NET: Fracture](https://github.com/fractureio/fracture): A high-performance socket I/O message pipeline library.
- [.NET: SuperSocket](http://www.supersocket.net/): SuperSocket 是一个轻量级, 跨平台而且可扩展的 .Net/Mono Socket 服务器程序框架。你无须了解如何使用 Socket, 如何维护 Socket 连接和 Socket 如何工作，但是你却可以使用 SuperSocket 很容易的开发出一款 Socket 服务器端软件，例如游戏服务器，GPS 服务器, 工业控制服务和数据采集服务器等等。

## Thread & Coroutine

- [.NET: Wintellect PowerThreading](https://github.com/Wintellect/PowerThreading): Jeffrey Richter's Power Threading Library

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

- [.NET: BouncyCastle](https://bouncycastle.org/) - Together with the .Net System.Security.Cryptography, the reference implementation for cryptographic algorithms on the CLR.
- [.NET: HashLib](http://hashlib.codeplex.com/) - HashLib is a collection of nearly all hash algorithms you've ever seen, it supports almost everything and is very easy to use
- [.NET: libsodium-net](https://github.com/adamcaudill/libsodium-net) - libsodium for .NET - A secure cryptographic library
- [.NET: StreamCryptor](https://github.com/bitbeans/StreamCryptor) - Stream encryption & decryption with libsodium and protobuf

## Compression

- [.NET: SharpCompress](https://github.com/adamhathcock/sharpcompress) - SharpCompress is a compression library for .NET/Mono/Silverlight/WP7 that can unrar, un7zip, unzip, untar unbzip2 and ungzip with forward-only reading and file random access APIs. Write support for zip/tar/bzip2/gzip are implemented
- [.NET: DotNetZip.Semverd](https://github.com/haf/DotNetZip.Semverd) - An open-source project that delivers a .NET library for handling ZIP files, and some associated tools. (fork of Unmaintained DotNetZip)
- [.NET: SharpZipLib](http://icsharpcode.github.io/SharpZipLib/) - a Zip, GZip, Tar and BZip2 library written entirely in C# for the .NET platform

## Profiler

- [.NET: MiniProfiler](http://miniprofiler.com/): A simple but effective mini-profiler for .NET and Ruby
- [.NET: Glimpse](http://getglimpse.com/): Providing real time diagnostics & insights to the fingertips of hundreds of thousands of developers daily
- [.NET: metrics-net](https://github.com/danielcrenna/metrics-net): Capturing CLR and application-level metrics. So you know what's going on.
- [.NET: Metrics.NET](https://github.com/etishor/Metrics.NET): The Metrics.NET library provides a way of instrumenting applications with custom metrics (timers, histograms, counters etc) that can be reported in various ways and can provide insights on what is happening inside a running application.

## Data Access

- [.NET: StackExchange.Redis](https://github.com/StackExchange/StackExchange.Redis): a high performance general purpose redis client for .NET languages (C# etc)
- [.NET: SolrNet](https://github.com/mausch/SolrNet): SolrNet is an Apache Solr client for .NET
- [.NET: EasyNetQ](https://github.com/EasyNetQ/EasyNetQ): An easynet to use .NET API for RabbitMQ, not offical rabbitmq .net client
- [.NET: DbUtility](https://github.com/Ivony/DbUtility):  a light database access tool
- [.NET: Drapper](https://github.com/StackExchange/dapper-dot-net): a simple object mapper for .Net
- [.NET: Entity Framework](https://github.com/aspnet/EntityFramework): Microsoft's recommended data access technology for new applications in .NET.
- [.NET: MyBatis](https://mybatis.github.io/): MyBatis is a first class persistence framework with support for custom SQL, stored procedures and advanced mappings. MyBatis eliminates almost all of the JDBC code and manual setting of parameters and retrieval of results. MyBatis can use simple XML or Annotations for configuration and map primitives, Map interfaces and Java POJOs (Plain Old Java Objects) to database records.
- [.NET: ServiceStack.OrmLite](https://github.com/ServiceStack/ServiceStack.OrmLite): Fast, Simple, Typed ORM for .NET
- [.NET: NHibernate](http://nhibernate.info/): NHibernate is a mature, open source object-relational mapper for the .NET framework. It's actively developed, fully featured and used in thousands of successful projects.
- [.NET: fluent-nhibernate](https://github.com/jagregory/fluent-nhibernate): Fluent, XML-less, compile safe, automated, convention-based mappings for NHibernate. Get your fluent on.

## Serialization & Deserialization

- [.NET: Jil](https://github.com/kevin-montrose/Jil): Fast .NET JSON (De)Serializer, Built On Sigil
- [.NET: ServiceStack.Text](https://github.com/ServiceStack/ServiceStack.Text): .NET's fastest JSON, JSV and CSV Text Serializers
- [.NET: Json.net](http://www.newtonsoft.com/json): Popular high-performance JSON framework for .NET
- [.NET: fastjson](https://fastjson.codeplex.com/): Smallest, fastest polymorphic JSON serializer

## Command Line

- [.NET: Command Line Parser](https://github.com/gsscoder/commandline) - The Command Line Parser Library offers to CLR applications a clean and concise API for manipulating command line arguments and related tasks
- [.NET: Fluent Command Line Parser](https://github.com/fclp/fluent-command-line-parser) - A simple, strongly typed .NET C# command line parser library using a fluent easy to use interface
- [.NET: Power Args](https://github.com/adamabdelhamed/PowerArgs) - PowerArgs converts command line arguments into .NET objects that are easy to program against. It also provides a ton of optional capabilities such as argument validation, auto generated usage, tab completion, and plenty of extensibility

## Math

- [.NET: Math.NET](https://www.mathdotnet.com/)
	- [Math.NET Numerics: numerical computing](http://numerics.mathdotnet.com/): Math.NET Numerics aims to provide methods and algorithms for numerical computations in science, engineering and every day use. Covered topics include special functions, linear algebra, probability models, random numbers, interpolation, integration, regression, optimization problems and more.
	- [Math.NET Symbolics: computer algebra](http://symbolics.mathdotnet.com/): Math.NET Symbolics is a basic open source computer algebra library for .Net and Mono written in F#.
	- [Math.NET Filtering: signal processing](http://filtering.mathdotnet.com/): Filtering aims to provide a toolkit for digital signal processing, offering an infrastructure for digital filter design, applying those filters to data streams using data converters, as well as digital signal generators.
	- [Math.NET Spatial](http://spatial.mathdotnet.com/): Math.NET Spatial is aiming to become a geometry library for .Net and Mono.

## Image Processing

- [.NET: ImageProcessor](http://imageprocessor.org/): ImageProcessor is a collection of lightweight libraries written in C# that allows you to manipulate images on-the-fly using .NET 4.5+

## Computer Vision

- [.NET: AForge.NET](http://www.aforgenet.com/): AForge.NET is a C# framework designed for developers and researchers in the fields of Computer Vision and Artificial Intelligence - image processing, neural networks, genetic algorithms, machine learning, robotics, etc.

## Authentication & Authorization

- [.NET: ASP.NET Identity](https://aspnetidentity.codeplex.com/) - New membership system for ASP.NET applications
- [.NET: DotNetOpenAuth](https://github.com/DotNetOpenAuth/DotNetOpenAuth) - A C# implementation of the OpenID, OAuth and InfoCard protocols
- [.NET: IdentityModel](https://github.com/IdentityModel) - Helper library for identity & access control in .NET 4.5 and MVC4/Web API.
- [.NET: IdentityServer](https://github.com/IdentityServer) - Extensible OAuth2 and OpenID Connect provider framework.
- [.NET: OAuth](https://github.com/danielcrenna/oauth) - A very lightweight library for generating OAuth 1.0a signatures written in C#

## Mail

- [.NET: FluentEmail](https://github.com/lukencode/FluentEmail): A Fluent Wrapper for System.Net.Mail with razor templating support.
- [.NET: MailKit](https://github.com/jstedfast/MailKit): A complete cross-platform mail stack including IMAP, POP3, SMTP, authentication and more. Built on top of MimeKit.
- [.NET: MimeKit](https://github.com/jstedfast/MimeKit): A cross-platform .NET MIME creation and parser library with support for S/MIME, PGP, TNEF and Unix mbox spools.
- [.NET: MailSystem.NET](https://mailsystem.codeplex.com/): MailSystem is a suite of .NET components that provide users with an extensive set of email tools. MailSystem provides full support for SMTP, POP3, IMAP4, NNTP, MIME, S/MIME, OpenPGP, DNS, vCard, vCalendar, Anti-Spam (Bayesian , RBL, DomainKeys), Queueing, Mail Merge and WhoIs. If you wish to use this code in non GPLv3 software, you must acquire a commercial license. Please send your request to the coordinator of this project.

## State Machine

- [.NET: Stateless](https://github.com/nblumhardt/stateless) - Create state machines and lightweight state machine-based workflows directly in .NET code
- [.NET: Automatonymous](https://github.com/MassTransit/Automatonymous) - A state machine library for .Net - allows you to write fluent style state machines

## .NET Interoperability

- [.NET: CppSharp](https://github.com/mono/CppSharp) - Tools to surface C++ APIs to C#
- [.NET: Sharpen](https://github.com/mono/sharpen) - Sharpen is an Eclipse plugin created by db4o that allows you to convert your Java project into C#
- [.NET: CXXI](https://github.com/mono/cxxi) - C++ interop framework

## Windows Services

- [.NET: Topshelf](http://topshelf-project.com/): Put Your Apps on the Topshelf

## Misc Libraries

- [.NET: AutoMapper](http://automapper.org/): a simple little library built to solve a deceptively complex problem - getting rid of code that mapped one object to another.
- [.NET: UrlRewriter](https://github.com/sethyates/urlrewriter): UrlRewriter.NET is an open-source, light-weight, highly configurable URL rewriting component for ASP.NET 1.1 – 4.0.
- [.NET: Fast Reflection Library](http://fastreflectionlib.codeplex.com/): FastReflectionLib provide the same as part of the refection features like executing method dynamically but give simple and faster implementations. It can be use as the foundation of reflection-based scenarios such as ORM framework.
- [.NET: FluentValidation](https://github.com/JeremySkinner/FluentValidation): A small validation library for .NET that uses a fluent interface and lambda expressions for building validation rules. Written by Jeremy Skinner (http://www.jeremyskinner.co.uk) and licensed under Apache 2.
- [.NET: Html Agility Pack](https://htmlagilitypack.codeplex.com/): This is an agile HTML parser that builds a read/write DOM and supports plain XPATH or XSLT (you actually don't HAVE to understand XPATH nor XSLT to use it, don't worry...). It is a .NET code library that allows you to parse "out of the web" HTML files. The parser is very tolerant with "real world" malformed HTML. The object model is very similar to what proposes System.Xml, but for HTML documents (or streams).
- [.NET: Base Class Libraries](https://bcl.codeplex.com/): The Base Class Libraries site hosts samples, previews, and prototypes from the BCL team.
- [.NET: CommonLibrary.NET](https://commonlibrarynet.codeplex.com/): A collection of very reusable code and components in C# 4.0 ranging from ActiveRecord, Csv, Command Line Parsing, Configuration, Validation, Logging, Collections, Authentication, and much more. This is ideal for C# developer looking for a Utility library, Java developers looking for a C# version of Java Commons.
- [.NET: Craig-s-Utility-Library](http://jacraig.github.io/Craig-s-Utility-Library/): With .Net we have a number of built in classes and functions to help make a programmer's life easier, but let's face facts, they didn't think of everything. Craig's Utility Library tries to fill in some of those gaps (or at least the ones that I've run into). It comes with a couple hundred extension methods, built in data types such as a BTree, priority queue, ring buffer, etc. And that's just the DataTypes namespace. When you add it all up, Craig's Utility Library is one of the largest set of utilities for .Net out there.
- [.NET: Wintellect's Power Collections for .NET](http://powercollections.codeplex.com/): Power Collections makes heavy use of .NET Generics. The goal of the project is to provide generic collection classes that are not available in the .NET framework. Some of the collections included are the Deque, MultiDictionary, Bag, OrderedBag, OrderedDictionary, Set, OrderedSet, and OrderedMultiDictionary.
- [.NET: Humanizer](https://github.com/MehdiK/Humanizer): Humanizer meets all your .NET needs for manipulating and displaying strings, enums, dates, times, timespans, numbers and quantities
- [.NET: Sigil](https://github.com/kevin-montrose/Sigil): A fail-fast validating helper for .NET CIL generation
- [.NET: Shielded](https://github.com/jbakic/Shielded): A strict and mostly lock-free Software Transactional Memory (STM) for .NET
- [.NET: NodaTime](https://github.com/nodatime/nodatime): A better date and time API for .NET
- [.NET: FastFileFinder](https://github.com/Wintellect/FastFileFinder): Find files and directory names FAST!
