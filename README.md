# 说明

这是一本手册，帮助你使用（但不仅限于）dotNET开发更好的应用。

备注：
- [website-attack-and-defense.md](./website-attack-and-defense.md): 常见的网络攻击手段和防御方法
- [magic-fsharp](./magic-fsharp/md): F#学习资料

-------------------------------------------------------------------------------

# Books

- [CLR via C#](http://book.douban.com/subject/4924165/)
- [C# in Depth](http://book.douban.com/subject/3133747/) - [图书官网](http://csharpindepth.com/)
- [Threading in C#](http://www.albahari.com/threading/)
- [Concurrency in C# Cookbook](http://book.douban.com/subject/25899958/)
- [Windows并发编程指南](http://book.douban.com/subject/4214617/)

-------------------------------------------------------------------------------

# Code Style Guide

- [NET设计规范：约定、惯用法与模式](http://book.douban.com/subject/4231292/)
- [C# 3.0, C# 4.0 and C# 5.0 Coding Guidelines](http://csharpguidelines.codeplex.com/)
- [Style guides for Google-originated open-source projects](https://github.com/google/styleguide)
- [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)

-------------------------------------------------------------------------------

# Foundation, Organization, Specification

## Organization

- [.NET Foundation](http://www.dotnetfoundation.org)
- [patterns & practices](https://msdn.microsoft.com/en-us/library/ff921345.aspx)
- [ServiceStack](https://servicestack.net/)
- [StackExchange](https://github.com/StackExchange)
- [Castle Projects](http://www.castleproject.org)
- [Mono Projects](https://github.com/mono)

## Specification

- [OWIN - Open Web Interface for .NET](http://owin.org/)
- [OData](http://odata.github.io/): OData is an OASIS standard for creating and consuming RESTful APIs.
- HTTP
    - [HTTP/2 Protocol](http://http2.github.io/): HTTP/2 is a replacement for how HTTP is expressed “on the wire.” It is not a ground-up rewrite of the protocol; HTTP methods, status codes and semantics are the same, and it should be possible to use the same APIs as HTTP/1.x (possibly with some small additions) to represent the protocol.
    - [HTTP/2 explained](http://daniel.haxx.se/http2/): http2 explained describes the protocol HTTP/2 at a technical and protocol level. Background, the protocol, the implementations and the future. Written by Daniel Stenberg.
- Data Exchange Format
    - [Portocol Buffer](https://developers.google.com/protocol-buffers/): Protocol buffers are Google's language-neutral, platform-neutral, extensible mechanism for serializing structured data – think XML, but smaller, faster, and simpler. 
    - [Message Pack](http://msgpack.org/): MessagePack is an efficient binary serialization format. It lets you exchange data among multiple languages like JSON. But it's faster and smaller. Small integers are encoded into a single byte, and typical short strings require only one extra byte in addition to the strings themselves.
    - [Apache Thrift](http://thrift.apache.org/): Thrift源于大名鼎鼎的facebook之手，在2007年facebook提交Apache基金会将Thrift作为一个开源项目，对于当时的facebook来说创造thrift是为了解决facebook系统中各系统间大数据量的传输通信以及系统之间语言环境不同需要跨平台的特性。所以thrift可以支持多种程序语言，例如: C++, C#, Cocoa, Erlang Haskell, Java, Ocami, Perl, PHP, Python, Ruby, Smalltalk. 在多种不同的语言之间通信thrift可以作为二进制的高性能的通讯中间件，支持数据(对象)序列化和多种类型的RPC服务。Thrift适用于程序对程序静态的数据交换，需要先确定好他的数据结构，他是完全静态化的，当数据结构发生变化时，必须重新编辑IDL文件，代码生成，再编译载入的流程，跟其他IDL工具相比较可以视为是Thrift的弱项，Thrift适用于搭建大型数据交换及存储的通用工具，对于大型系统中的内部数据传输相对于JSON和xml无论在性能、传输大小上有明显的优势。
    - [Apache Avro](http://avro.apache.org/): Apache Avro™ is a data serialization system.
    - [Cap’n Proto](https://capnproto.org/index.html): Cap’n Proto is an insanely fast data interchange format and capability-based RPC system. Think JSON, except binary. Or think Protocol Buffers, except faster. In fact, in benchmarks, Cap’n Proto is INFINITY TIMES faster than Protocol Buffers.
    - [Microsoft bond](https://github.com/Microsoft/bond): Bond is a cross-platform framework for working with schematized data. It supports cross-language de/serialization and powerful generic mechanisms for efficiently manipulating data. Bond is broadly used at Microsoft in high scale services.
    - [JSON](http://json.org/): JSON (JavaScript Object Notation) is a lightweight data-interchange format. It is easy for humans to read and write. It is easy for machines to parse and generate. It is based on a subset of the JavaScript Programming Language, Standard ECMA-262 3rd Edition - December 1999. JSON is a text format that is completely language independent but uses conventions that are familiar to programmers of the C-family of languages, including C, C++, C#, Java, JavaScript, Perl, Python, and many others. These properties make JSON an ideal data-interchange language.
        - [JSON Schema](http://json-schema.org/)
        - [JSON Schema Generator](http://jsonschema.net/)

-------------------------------------------------------------------------------

# Projects about Development

## CLR Framework

- [.NET Framewrok](https://msdn.microsoft.com/en-us/vstudio/aa496123.aspx)
- [.NET Core](http://dotnet.github.io/core/): A general purpose managed framework
- [Mono](http://www.mono-project.com/): Cross platform, open source .NET framework

## Web Frameworks/Application Frameworks

- [ASP.net MVC 6](https://github.com/aspnet/Mvc): Model view controller framework for building dynamic web sites with clean separation of concerns, including the merged MVC, Web API, and Web Pages, Razor.
- [ASP.net MVC 5](http://aspnetwebstack.codeplex.com/): ASP.NET MVC gives you a powerful, patterns-based way to build dynamic websites that enables a clean separation of concerns and that gives you full control over markup for enjoyable, agile development. ASP.NET MVC includes many features that enable fast, TDD-friendly development for creating sophisticated applications that use the latest web standards.
- [ASP.net Web API 2](http://www.asp.net/web-api): ASP.NET Web API is a framework that makes it easy to build HTTP services that reach a broad range of clients, including browsers and mobile devices. ASP.NET Web API is an ideal platform for building RESTful applications on the .NET Framework.
- [ServiceStack](https://github.com/ServiceStack/ServiceStack): Simple, Fast, Versatile and full-featured Services Framework
- [Nancy](http://nancyfx.org/): Lightweight, low-ceremony, framework for building HTTP based services on .Net and Mono
- [Apworks](https://github.com/daxnet/Apworks): Apworks is a flexible, scalable, configurable and efficient .NET based application development framework that helps software developers to easily build enterprise applications by applying either Classic Layering or Command-Query Responsibility Segregation (CQRS) architectural patterns.

## Template Engine

- [RazorEngine](https://github.com/Antaris/RazorEngine): Open source templating engine based on Microsoft's Razor parsing engine
- [Nustache](https://github.com/jdiamond/Nustache): Logic-less templates for .NET
- [dotliquid](http://dotliquidmarkup.org/): a templating system ported to the .net framework from Ruby’s Liquid Markup.
- [StringTemplate](http://www.stringtemplate.org/): StringTemplate is a java template engine (with ports for C#, JavaScript, Python) for generating source code, web pages, emails, or any other formatted text output. StringTemplate is particularly good at code generators, multiple site skins, and internationalization / localization. StringTemplate also powers ANTLR.

## Web Servers & Hosts

- [Katana](http://katanaproject.codeplex.com/): As Web application development takes its next evolutionary step into the world of cloud computing, project Katana provides the underlying set of components to ASP.NET applications, enabling them to be flexible, portable, lightweight, and provide better performance – put another way, project Katana cloud optimizes your ASP.NET applications.
- [Nowin](https://github.com/Bobris/Nowin): Fast and scalable Owin Web Server in pure .Net 4.5 (it does not use HttpListener). Current status is usable for testing, not for production, nobody did any security review, you have been warned. On Windows speed is better than NodeJs and in some cases even better than HttpListener.
- [Jexus](http://www.jexus.org/): 強勁、堅固、免費、易用的Linux ASP.NET服務器
- [XSP](https://github.com/mono/xsp): Mono's ASP.NET hosting server. This module includes an Apache Module, a FastCGI module that can be hooked to other web servers as well as a standalone server used for testing (similar to Microsoft's Cassini)
- [EmbedIO](https://github.com/unosquare/embedio): A tiny, cross-platform, module based web server
- [Nginx](http://wiki.nginx.org/Main): a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
- [Tengine](http://tengine.taobao.org/): Tengine是由淘宝网发起的Web服务器项目。它在Nginx的基础上，针对大访问量网站的需求，添加了很多高级功能和特性。Tengine的性能和稳定性已经在大型的网站如淘宝网，天猫商城等得到了很好的检验。它的最终目标是打造一个高效、稳定、安全、易用的Web平台。

## WebSocket

- [SignalR](https://github.com/SignalR/SignalR): Library for ASP.NET developers that makes it incredibly simple to add real-time web functionality to your applications
- [Fleck](https://github.com/statianzo/Fleck) - Fleck is a WebSocket server implementation in C#. Branched from the Nugget project
- [Websocket-Sharp](https://github.com/sta/websocket-sharp) - A C# implementation of the WebSocket protocol client and server
- [WebSocket4NET](https://websocket4net.codeplex.com/) - WebSocket client for .NET 2.0+, Xamarin, Mono, Silverlight, Windows Phone, & WinRT

## Network

- [Fracture](https://github.com/fractureio/fracture): A high-performance socket I/O message pipeline library.
- [SuperSocket](http://www.supersocket.net/): SuperSocket 是一个轻量级, 跨平台而且可扩展的 .Net/Mono Socket 服务器程序框架。你无须了解如何使用 Socket, 如何维护 Socket 连接和 Socket 如何工作，但是你却可以使用 SuperSocket 很容易的开发出一款 Socket 服务器端软件，例如游戏服务器，GPS 服务器, 工业控制服务和数据采集服务器等等。
- [RestSharper](http://restsharp.org/): Simple REST and HTTP API Client for .NET

## Authentication && Authorization

- [DotNetOpenAuth](https://github.com/DotNetOpenAuth/DotNetOpenAuth) - A C# implementation of the OpenID, OAuth and InfoCard protocols

## Data Access

- [StackExchange.Redis](https://github.com/StackExchange/StackExchange.Redis): a high performance general purpose redis client for .NET languages (C# etc)
- [SolrNet](https://github.com/mausch/SolrNet): SolrNet is an Apache Solr client for .NET
- [EasyNetQ](https://github.com/EasyNetQ/EasyNetQ): An easynet to use .NET API for RabbitMQ, not offical rabbitmq .net client
- [DbUtility](https://github.com/Ivony/DbUtility):  a light database access tool

**ORM framework**

- [Drapper](https://github.com/StackExchange/dapper-dot-net): a simple object mapper for .Net
- [Entity Framework](https://github.com/aspnet/EntityFramework): Microsoft's recommended data access technology for new applications in .NET.
- [MyBatis](https://mybatis.github.io/): MyBatis is a first class persistence framework with support for custom SQL, stored procedures and advanced mappings. MyBatis eliminates almost all of the JDBC code and manual setting of parameters and retrieval of results. MyBatis can use simple XML or Annotations for configuration and map primitives, Map interfaces and Java POJOs (Plain Old Java Objects) to database records.
- [ServiceStack.OrmLite](https://github.com/ServiceStack/ServiceStack.OrmLite): Fast, Simple, Typed ORM for .NET
- [nhibernate](http://nhibernate.info/): NHibernate is a mature, open source object-relational mapper for the .NET framework. It's actively developed, fully featured and used in thousands of successful projects.
- [fluent-nhibernate](https://github.com/jagregory/fluent-nhibernate): Fluent, XML-less, compile safe, automated, convention-based mappings for NHibernate. Get your fluent on.

## Serialization & Deserialization

- [Jil](https://github.com/kevin-montrose/Jil): Fast .NET JSON (De)Serializer, Built On Sigil
- [ServiceStack.Text](https://github.com/ServiceStack/ServiceStack.Text): .NET's fastest JSON, JSV and CSV Text Serializers
- [Json.net](http://www.newtonsoft.com/json): Popular high-performance JSON framework for .NET
- [fastjson](https://fastjson.codeplex.com/): Smallest, fastest polymorphic JSON serializer

## Windows services

- [Topshelf](http://topshelf-project.com/): Put Your Apps on the Topshelf

## Schedule Task

- [Quartz](http://quartz-scheduler.org/): Quartz is a richly featured, open source job scheduling library that can be integrated within virtually any Java application - from the smallest stand-alone application to the largest e-commerce system. Quartz can be used to create simple or complex schedules for executing tens, hundreds, or even tens-of-thousands of jobs; jobs whose tasks are defined as standard Java components that may execute virtually anything you may program them to do. The Quartz Scheduler includes many enterprise-class features, such as support for JTA transactions and clustering.
- [QuartzNet](https://github.com/quartznet/quartznet): Quartz.NET is a pure .NET library written in C# and is a port of very popular open source Java job scheduling framework, Quartz.
- [FluentScheduler](https://github.com/jgeurts/FluentScheduler): A task scheduler that uses fluent interface to configure schedules. Useful for running cron jobs/automated tasks from your application.
- [Hangfire](https://github.com/HangfireIO/Hangfire): Incredibly easy way to perform fire-and-forget, delayed and recurring tasks inside ASP.NET applications
- [Gearman](http://gearman.org/): Gearman provides a generic application framework to farm out work to other machines or processes that are better suited to do the work. It allows you to do work in parallel, to load balance processing, and to call functions between languages. It can be used in a variety of applications, from high-availability web sites to the transport of database replication events.
- [schedulix - open source enterprise job scheduling](https://github.com/schedulix/schedulix): schedulix is an open source enterprise job scheduling system.
- [resque-schedule](https://github.com/resque/resque-scheduler): A light-weight job scheduling system built on top of resque

## State Machine

- [Stateless](https://github.com/nblumhardt/stateless) - Create state machines and lightweight state machine-based workflows directly in .NET code
- [Automatonymous](https://github.com/MassTransit/Automatonymous) - A state machine library for .Net - allows you to write fluent style state machines

## Profiler

- [MiniProfiler](http://miniprofiler.com/): A simple but effective mini-profiler for .NET and Ruby
- [Glimpse](http://getglimpse.com/): Providing real time diagnostics & insights to the fingertips of hundreds of thousands of developers daily
- [metrics-net](https://github.com/danielcrenna/metrics-net): Capturing CLR and application-level metrics. So you know what's going on.

## Interoperability

- [CppSharp](https://github.com/mono/CppSharp) - Tools to surface C++ APIs to C#
- [Sharpen](https://github.com/mono/sharpen) - Sharpen is an Eclipse plugin created by db4o that allows you to convert your Java project into C#
- [CXXI](https://github.com/mono/cxxi) - C++ interop framework

## IoC

- [Castle Windsor](https://github.com/castleproject/Windsor) - Castle Windsor is best of breed, mature Inversion of Control container available for .NET and Silverlight
- [Unity](https://unity.codeplex.com/) - Lightweight extensible dependency injection container with support for constructor, property, and method call injection
- [Autofac](https://github.com/autofac/Autofac) - An addictive .NET IoC container
- [Ninject](https://github.com/ninject/ninject) - The ninja of .net dependency injectors
- [StructureMap](https://structuremap.github.io/) - The original IoC/DI Container for .Net
- [Spring.Net](https://github.com/spring-projects/spring-net) - Spring.NET is an open source application framework that makes building  enterprise .NET applications easier
- [LightInject](https://github.com/seesharper/LightInject) - A ultra lightweight IoC container
- [TinyIoC](https://github.com/grumpydev/TinyIoC) - Single-file, easy and cross-platform IoC container

## Logging

- [Essential Diagnostics](http://essentialdiagnostics.codeplex.com/) - Extends the inbuilt features of System.Diagnostics namespace to provide flexible logging
- [NLog](https://github.com/nlog/NLog/) - NLog - Advanced .NET and Silverlight Logging
- [Logary](http://logary.github.io/) - Logary is a high performance, multi-target logging, metric, tracing and health-check library for mono and .Net. .Net's answer to DropWizard. Supports many targets, built for micro-services.
- [Log4Net](https://logging.apache.org/log4net/) - The Apache log4net library is a tool to help the programmer output log statements to a variety of output targets
- [Serilog](https://github.com/serilog/serilog) - A no-nonsense logging library for the NoSQL era. Combines the best of traditional and structured diagnostic logging in an easy-to-use package.
- [StackExchange.Exceptional](https://github.com/NickCraver/StackExchange.Exceptional) - Error handler used for the Stack Exchange network

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

## Manipulate Documents

- [NPOI](https://github.com/tonyqus/npoi): NPOI 是 POI 项目的 .NET 版本。POI是一个开源的Java读写Excel、WORD等微软OLE2组件文档的项目。NPOI让.NET平台拥有了一个比较完善的读写Excel的工具。使用量非常广泛，应该是开源的.NET Excel读写工具中曝光度最高的一个吧，没有之一。
- [NPOI扩展—NPOI.CSS](https://github.com/qihangnet/npoi.css): NPOI.CSS是一个可以在使用NPOI时用类CSS的方法设置单元格样式的NPOI扩展，只支持.NET4及以上版本的项目。这个扩展是为了方便在使用的时候设置单元格及其相关格式样式，可以使用类似Css的方式，非常给力。
- [yjinglee.office](https://github.com/YJingLee/yjinglee.office): yjinglee.office用于.Net平台下的Excel操作，主要封装NPOI对外提供更简单实用的API，提供以下功能点：1.读取Excel数据转换成对象集合, 2.写入集合到Excel，并提供可以Excel样式定义
- [Epplus](http://epplus.codeplex.com/): Epplus是一个使用Open Office XML（Xlsx）文件格式，读写Excel 2007/2010文件的开源组件。和NPOI相比，它更早的支持了Xlsx格式，而NPOI支持Excel 2003更好，现在新版本的NPOI也开始支持Xlsx了。支持的范围也很广，例如：单元格合并，单元格样式，图表(这个NPOI目前还不是很好)，表格，数据验证，公式，VBA等等。
- [LinqToExcel](https://github.com/paulyoder/LinqToExcel): LinqToExcel是一个.NET平台下开源项目，它主要实现了LINQ的语法查询Excel电子表格。类型之前的LINQToXXX如果你是LINQ语法糖爱好者那最适合你。
- [NetOffice](http://netoffice.codeplex.com/): NetOffice组件比较特别，是一个操作Office的强大组件，包括处理Office, Excel, Word, Outlook, PowerPoint, Access, Project, Visio等，所以支持非常全面。但是这个组件并不是完全单独写的，而是调用Microsoft Office的互操作程序集以及VSTO，也就是进行了一个深度的封装，从而让你不需要安装这些东西，只需要拷贝相应的程序集就可以了。
- [Word文档读写工具Docx](http://docx.codeplex.com/): DocX is a .NET library that allows developers to manipulate Word 2007/2010/2013 files, in an easy and intuitive manor. DocX is fast, lightweight and best of all it does not require Microsoft Word or Office to be installed.
- [iText](http://itextpdf.com/product/itext): 打开这个[链接](http://itextpdf.com/functionality)，图里面已经说得很清楚了。
- [PDFSharp](http://www.pdfsharp.net/): PDFsharp is a .NET library for processing PDF file. You create PDF pages using drawing routines known from GDI+. Almost anything that can be done with GDI+ will also work with PDFsharp. Only basic text layout is supported by PDFsharp, and page breaks are not created automatically. The same drawing routines can be used for screen, PDF, or meta files.
- [MigraDoc](http://www.pdfsharp.net/): MigraDoc is a document generator. It supports almost anything you find in any good word processor. You just add paragraphs, tables, charts, arrange all this in sections, use bookmarks to create links, tables of contents, indexes, etc. MigraDoc will do the layout creating page breaks as needed. MigraDoc will create PDF, XPS, or RTF documents.

## Manipulate Texts

- [文件差异比较diffplex](https://github.com/mmanela/diffplex): diffplex是一个开源的C#文本差异比较软件。支持.NET 4.0, Silverlight 5.0, Windows 8.0, Windows Phone 8.0, Windows Phone Appx 8.1等环境。

## Report

- [ExcelReport报表引擎](https://github.com/hanzhaoxin/ExcelReport): ExcelReport是一款基于NPOI开发的报表引擎组件。它基于关注点分离的理念，将数据与样式、格式分离。让模板承载样式、格式等NPOI不怎么擅长且实现繁琐的信息，结合NPOI对数据的处理的优点将Excel报表的生成化繁为简。同时，对报表组成的基本元素进行了抽象，进一步简化了Excel报表的生成过程。
- [PDFReport](http://pdfreport.codeplex.com/): PdfReport 是一个支持code-first的报表引擎，建立在开源项目iTextSharp和 EPPlus基础上。支持.net 3.5以上
- [ReportGenerator](https://github.com/danielpalme/ReportGenerator): ReportGenerator可以将OpenCover, PartCover, Visual Studio 或者NCover生成的XML报表转换为可读性更加好的格式。上面这几个工具都是代码覆盖率分析工具。转换后的报表有以下格式：1.HTML, HTMLSummary, 2.XML, XMLSummary, 3.Latex, LatexSummary, 4.TextSummary, 5.Custom reports
- [BusyReports - Advanced Report delivery with SQL Server Reporting Services SSRS](http://busyreports.codeplex.com/): BusyReports is an easy to use application to produce reports from the SSRS web services. It is an alternative to the data driven subscriptions of SQL Server.
- [Seal Report](http://sealreport.codeplex.com/): Seal Report offers a complete framework for producing every day reports and dashboards from any database.

## Tools

- [CS-Script](http://www.csscript.net/index.html): CS-Script is a CLR (Common Language Runtime) based scripting system which uses ECMA-compliant C# as a programming language. CS-Script currently targets Microsoft implementation of CLR (.NET 2.0/3.0/3.5/4.0/4.5) with full support on Mono.
- [Scriptcs](http://scriptcs.net/): Unleash your C# from Visual Studio.
- [dotPeek](https://www.jetbrains.com/decompiler/): Free .NET Decompiler and Assembly Browser
- [FastFileFinder](https://github.com/Wintellect/FastFileFinder): Find files and directory names FAST!

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
- [ImageProcessor](http://imageprocessor.org/): ImageProcessor is a collection of lightweight libraries written in C# that allows you to manipulate images on-the-fly using .NET 4.5+
- [Hugin](http://sourceforge.net/projects/hugin): Panorama photo stitcher
- [Luminance HDR](http://sourceforge.net/projects/qtpfsgui): Complete solution for HDR photography
- $[Pano2VR && Object2VR](http://ggnome.com/): software for interactive panoramas and object movies.

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
- [ShouldBe](https://github.com/shouldly/shouldly): Should testing for .net - the way Asserting *Should* be!
- [Humanizer](https://github.com/MehdiK/Humanizer): Humanizer meets all your .NET needs for manipulating and displaying strings, enums, dates, times, timespans, numbers and quantities
- [Wintellect PowerThreading](https://github.com/Wintellect/PowerThreading): Jeffrey Richter's Power Threading Library

-------------------------------------------------------------------------------

# Projects about Distributed Architecture

## Distributed Application Framework

- [Microsoft Project Orleans](http://dotnet.github.io/orleans/): Orleans is a framework that provides a straightforward approach to building distributed high-scale computing applications, without the need to learn and apply complex concurrency or other scaling patterns.
- [akka.net](http://getakka.net/): a toolkit and runtime for building highly concurrent, distributed, and fault tolerant event-driven applications on .NET & Mono.
- [akka](http://akka.io/): Akka is a toolkit and runtime for building highly concurrent, distributed, and resilient message-driven applications on the JVM. The power of Akka is also available on the .NET Framework and Mono via the Akka.NET project.
- [Zyan Communication Framework](http://zyan.com.de/): Easy to use distributed application framework for .NET, Mono and Xamarin.Android.

## Distributed realtime computation system

- [Apache Storm](http://storm.apache.org/): Storm has many use cases: realtime analytics, online machine learning, continuous computation, distributed RPC, ETL, and more. Storm is fast: a benchmark clocked it at over a million tuples processed per second per node. It is scalable, fault-tolerant, guarantees your data will be processed, and is easy to set up and operate.
- [jstorm](https://github.com/alibaba/jstorm): JStorm is a distributed and fault-tolerant realtime computation system. Inspired by Apache Storm, JStorm has been completely rewritten in Java and provides many more enhanced features. JStorm has been widely used in many enterprise environments and proved robust and stable.
- [Twitter Heron](http://dl.acm.org/citation.cfm?id=2742788): 参考[Twitter发布新的大数据实时分析系统Heron](http://geek.csdn.net/news/detail/33750)
- [Apache Samza](http://samza.apache.org/): Apache Samza is a distributed stream processing framework. It uses Apache Kafka for messaging, and Apache Hadoop YARN to provide fault tolerance, processor isolation, security, and resource management.
- [Apache Kafka](http://kafka.apache.org/): Apache Kafka is publish-subscribe messaging rethought as a distributed commit log.

## Service Bus

- [MassTransit](http://masstransit-project.com/): Lean Service Bus for .NET
- [Rebus](https://github.com/rebus-org/Rebus): Rebus is a lean service bus implementation for .NET, similar in nature to NServiceBus and MassTransit, only leaner
- [NServiceBus](https://github.com/Particular): The most popular service bus for .NET
- [Shuttle-ESB](http://shuttle.github.io/shuttle-esb/): A highly configurable free open-source enterprise service bus that provides you with a mechanism to create Autonomous Business Components that are loosely coupled. This enables you to develop and deploy specific business functionality that can be independently versioned.
- [Rhino ESB](https://github.com/hibernating-rhinos/rhino-esb): Rhino Service Bus is a messaging framework that supports transactional, durable, reliable, distributed, asynchronous messaging. Rhino Service Bus currently supports two transports MSMQ and Rhino.Queues.

## Messsage Queue

- [RabbitMQ](http://www.rabbitmq.com/): RabbitMQ is a messaging broker - an intermediary for messaging. It gives your applications a common platform to send and receive messages, and your messages a safe place to live until received.
- [ZeroMQ](http://zeromq.org/): ZeroMQ (also known as ØMQ, 0MQ, or zmq) looks like an embeddable networking library but acts like a concurrency framework. It gives you sockets that carry atomic messages across various transports like in-process, inter-process, TCP, and multicast. You can connect sockets N-to-N with patterns like fan-out, pub-sub, task distribution, and request-reply. It's fast enough to be the fabric for clustered products. Its asynchronous I/O model gives you scalable multicore applications, built as asynchronous message-processing tasks. It has a score of language APIs and runs on most operating systems.
- [NetMQ](https://github.com/zeromq/netmq): NetMQ is 100% native C# port of ZeroMQ
- [beanstalkd](http://kr.github.io/beanstalkd/): Beanstalk is a simple, fast work queue. Its interface is generic, but was originally designed for reducing the latency of page views in high-volume web applications by running time-consuming tasks asynchronously.
- [Apache ActiveMQ](http://activemq.apache.org/): Apache ActiveMQ ™ is the most popular and powerful open source messaging and Integration Patterns server. Apache ActiveMQ is fast, supports many Cross Language Clients and Protocols, comes with easy to use Enterprise Integration Patterns and many advanced features while fully supporting JMS 1.1 and J2EE 1.4. Apache ActiveMQ is released under the Apache 2.0 License.
- [NSQ](https://github.com/bitly/nsq): NSQ is a realtime distributed messaging platform designed to operate at scale, handling billions of messages per day.

## Load Balance

- [LVS](http://www.linuxvirtualserver.org/): The Linux Virtual Server is a highly scalable and highly available server built on a cluster of real servers, with the load balancer running on the Linux operating system. The architecture of the server cluster is fully transparent to end users, and the users interact as if it were a single high-performance virtual server.
- [HAProxy](http://www.haproxy.org/): HAProxy is a free, very fast and reliable solution offering high availability, load balancing, and proxying for TCP and HTTP-based applications.
- [Nginx](http://wiki.nginx.org/Main): Nginx (pronounced engine-x) is a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
- [Pen](http://siag.nu/pen/): Pen is a load balancer for "simple" TCP-based protocols such as HTTP or SMTP. It allows several servers to appear as one to the outside. It automatically detects servers that are down and distributes clients among the available servers. This gives high availability and scalable performance.
- [Balance](http://www.inlab.de/balance.html): Balance is a simple but powerful generic TCP proxy with round-robin load balancing and failover mechanisms. Its behavior can be controlled at runtime using a simple command line syntax. Balance supports IPv6 on the listening side, which makes it a very useful tool for IPv6 migration of IPv4 only services and servers.
- [keepalived](http://www.keepalived.org/): Keepalived is a routing software written in C. The main goal of this project is to provide simple and robust facilities for loadbalancing and high-availability to Linux system and Linux based infrastructures.

## Reverse Proxy

- [Nginx](http://wiki.nginx.org/Main): Nginx (pronounced engine-x) is a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
- [Varnish](https://www.varnish-cache.org/): Varnish是一款高性能且开源的反向代理服务器和http加速器。与传统的Squid相比，Varnish具有性能更高、速度更快、管理更方便 等诸多优点。作者Poul-Henning Kamp是FreeBSD的内核开发者之一。Varnish采用全新的软件体系架构，和现在的硬件提交配合紧密。在1975年时，储存媒介只有两种：内存 与硬盘。但现在计算 机系统的内存除了主存外，还包括了cpu内的L1、L2，甚至有L3快取。硬盘上也有自己的快取装置，因此squid cache自行处理物件替换的架构不可能得知这些情况而做到最佳化，但操作系统可以得知这些情况，所以这部份的工作应该交给操作系统处理，这就是 Varnish cache设计架构。挪威最大的在线报纸Verdens Gang使用3台Varnish代替了原来的12台squid，性能居然比以前更好，这是Varnish最成功的应用案例。
- [Squid](http://www.squid-cache.org/): Squid is a caching proxy for the Web supporting HTTP, HTTPS, FTP, and more. It reduces bandwidth and improves response times by caching and reusing frequently-requested web pages. Squid has extensive access controls and makes a great server accelerator. It runs on most available operating systems, including Windows and is licensed under the GNU GPL.

## Distributed File System

- [FastDFS](https://code.google.com/p/fastdfs/): [FastDFS on Google Code](https://code.google.com/p/fastdfs/), FastDFS is an open source high performance distributed file system. It's major functions include: file storing, file syncing and file accessing, and design for high capacity and load balance.
- [mogilefs](https://github.com/mogilefs/): MogileFS is our open source distributed filesystem.
- [MooseFS](http://www.moosefs.org/): MooseFS is a fault tolerant, network distributed file system. It spreads data over several physical servers which are visible to the user as one resource. 
- [XtreeFS](http://xtreemfs.org/index.php): XtreemFS is a general purpose storage system and covers most storage needs in a single deployment. It is open-source, requires no special hardware or kernel modules, and can be mounted on Linux, Windows and OS X.
- [Ceph](http://ceph.com/): Ceph is a distributed object store and file system designed to provide excellent performance, reliability and scalability. - See more at: http://ceph.com/#sthash.46aGKE2z.dpuf
- [Taobao File System](http://tfs.taobao.org/): TFS（Taobao !FileSystem）是一个高可扩展、高可用、高性能、面向互联网服务的分布式文件系统，主要针对海量的非结构化数据，它构筑在普通的Linux机器集群上，可为外部提供高可靠和高并发的存储访问。TFS为淘宝提供海量小文件存储，通常文件大小不超过1M，满足了淘宝对小文件存储的需求，被广泛地应用在淘宝各项应用中。它采用了HA架构和平滑扩容，保证了整个文件系统的可用性和扩展性。同时扁平化的数据组织结构，可将文件名映射到文件的物理地址，简化了文件的访问流程，一定程度上为TFS提供了良好的读写性能。

-------------------------------------------------------------------------------

# Projects about Data Storage and Analysis

## Database

- [SQL Server](https://msdn.microsoft.com/en-us/library/bb545450.aspx)
- [PostgreSQL](http://www.postgresql.org/)
- [MySQL](http://www.mysql.com/)
- [MariaDB](http://mariadb.org/)
- [WebScaleSQL](http://webscalesql.org/)
- [SQLlite](http://www.sqlite.org/index.html)

## Cache

- [Redis](http://redis.io/): Redis is an open source, BSD licensed, advanced key-value cache and store. It is often referred to as a data structure server since keys can contain strings, hashes, lists, sets, sorted sets, bitmaps and hyperloglogs.
- [Memcached](http://memcached.org/): Free & open source, high-performance, distributed memory object caching system, generic in nature, but intended for use in speeding up dynamic web applications by alleviating database load. Memcached is an in-memory key-value store for small chunks of arbitrary data (strings, objects) from results of database calls, API calls, or page rendering. Memcached is simple yet powerful. Its simple design promotes quick deployment, ease of development, and solves many problems facing large data caches. Its API is available for most popular languages.
- [twemproxy](https://github.com/twitter/twemproxy): A fast, light-weight proxy for memcached and redis
- [shared cache](http://www.sharedcache.com/cms/homepage.aspx): high performance distributed and replication cache system built for .Net applications running in server farms.

## NoSQL Database

- [MongoDB](https://www.mongodb.org/)
- [TokuMX](http://www.tokutek.com/): High-Performance MongoDB
- [InfluxDB](https://influxdb.com/index.html): An open-source distributed time series database with no external dependencies.
- [RavenDB](http://ravendb.net/): A linq enabled document database for .NET

## Data Analytics

- [infobright community edition](https://www.infobright.com/)

## Search

- [Apache Solr](http://lucene.apache.org/solr/): Solr is the popular, blazing-fast, open source enterprise search platform built on Apache Lucene.
    - [mmseg4j-solr](https://github.com/chenlb/mmseg4j-solr): mmseg4j for lucene or solr analyzer
	- [mmseg4j-core](https://github.com/chenlb/mmseg4j-core): mmseg4j core MMSEG for java chinese analyzer
- [ElasticSearch](https://www.elastic.co/): elasticsearch 的目标是解决上面的所有问题以及更多。她是开源的（Apache2协议），分布式的，RESTful的，构建在Apache Lucene之上的的搜索引擎.
    - [elasticsearch-rtf](https://github.com/medcl/elasticsearch-rtf): elasticsearch中文发行版，针对中文集成了相关插件，并带有Demo，方便新手学习,或者在生产环境中直接使用
    - [elasticsearch-analysis-ik](https://github.com/medcl/elasticsearch-analysis-ik): The IK Analysis plugin integrates Lucene IK analyzer into elasticsearch, support customized dictionary.
    - [elasticsearch-analysis-mmseg](https://github.com/medcl/elasticsearch-analysis-mmseg): Mmseg Analysis for ElasticSearch
    - [elasticsearch-analysis-pinyin](https://github.com/medcl/elasticsearch-analysis-pinyin): The Pinyin Analysis plugin integrates Pinyin4j(http://pinyin4j.sourceforge.net/) module into elasticsearch.
- [Sphinx](http://sphinxsearch.com/): Sphinx Search 是由俄罗斯人Andrew Aksyonoff 开发的高性能全文搜索软件包，在GPL与商业协议双许可协议下发行。Sphinx is an open source full text search server, designed from the ground up with performance, relevance (aka search quality), and integration simplicity in mind. It's written in C++ and works on Linux (RedHat, Ubuntu, etc), Windows, MacOS, Solaris, FreeBSD, and a few other systems.
    - [sphinx-for-chinese](http://sphinx-search.com/): sphinx-for-chinese是一款专注于中文搜索的全文检索软件，在sphinx的基础上添加了中文处理模块并优化了中文搜索效果。
- [xunsearch](http://www.xunsearch.com/): 开源免费、高性能、多功能, 简单易用的专业全文检索技术方案
- [bleve](https://github.com/blevesearch/bleve): A modern text indexing library for go
- [Apache Nutch](http://nutch.apache.org/): Apache Nutch是一个用Java编写的开源网络爬虫。Apache Nutch对于Solr已经支持得很好，这大大简化了Nutch与Solr的整合。
- [Apache Tika](http://tika.apache.org/): The Apache Tika™ toolkit detects and extracts metadata and text from over a thousand different file types (such as PPT, XLS, and PDF). All of these file types can be parsed through a single interface, making Tika useful for search engine indexing, content analysis, translation, and much more.

## Recommender System

- [SUGGEST: Recommendation Engine](http://glaros.dtc.umn.edu/gkhome/suggest/overview): SUGGEST is a Top-N recommendation engine that implements a variety of recommendation algorithms. Top-N recommender systems, a personalized information filtering technology, are used to identify a set of N items that will be of interest to a certain user. In recent years, top-N recommender systems have been used in a number of different applications such to recommend products a customer will most likely buy; recommend movies, TV programs, or music a user will find enjoyable; identify web-pages that will be of interest; or even suggest alternate ways of searching for information.
- [easyrec](http://easyrec.org/): With the open source recommendation engine easyrec you can add recommendations to your website within minutes. easyrec is a web application written in Java that provides personalized recommendations using RESTful Web Services ready to be integrated in your web enabled applications.
- [MyMediaLite](https://github.com/zenogantner/MyMediaLite): recommender system library for the CLR (.NET)
- [LensKit](http://lenskit.org/): Open-Source Tools for Recommender Systems
- [Crab](http://muricoca.github.io/crab/): A Recommender Framework in Python

## Big Data

- [Hadoop and related projects](http://hadoop.apache.org/)
- [basho](http://basho.com/): Introducing the Basho Data Platform. The most powerful way to manage today’s active workloads for Big Data.

## Machine Learning and Data Science

- [Accord.NET](http://accord-framework.net/) - Machine learning framework combined with audio and image processing libraries (computer vision, computer audition, signal processing and statistics).
- [Accord.NET Extensions](https://github.com/dajuric/accord-net-extensions) - Advanced image processing and computer vision algorithms made as fluent extensions.
- [AForge.NET](http://www.aforgenet.com/) - Framework for developers and researchers in the fields of Computer Vision and Artificial Intelligence (image processing, neural networks, genetic algorithms, machine learning, robotics).
- [PredictionIO](https://prediction.io/): An open-source machine learning server for developers and data scientists to create predictive engines for production environments, with zero downtime training and deployment.
- [Apache Mahout](https://mahout.apache.org/): The Apache Mahout™ project's goal is to build an environment for quickly creating scalable performant machine learning applications.
- [Aerosolve - Airbnb](http://airbnb.io/aerosolve/): A machine learning package built for humans.
- [Caffe](http://caffe.berkeleyvision.org/): Caffe is a deep learning framework made with expression, speed, and modularity in mind. It is developed by the Berkeley Vision and Learning Center (BVLC) and by community contributors. Yangqing Jia created the project during his PhD at UC Berkeley. Caffe is released under the BSD 2-Clause license.
- [golearn](https://github.com/sjwhitworth/golearn): Machine Learning for Go
- [shogun](https://github.com/shogun-toolbox/shogun): The Shogun Machine learning toolbox provides a wide range of unified and efficient Machine Learning (ML) methods. The toolbox seamlessly allows to easily combine multiple data representations, algorithm classes, and general purpose tools. This enables both rapid prototyping of data pipelines and extensibility in terms of new algorithms. We combine modern software architecture in C++ with both efficient low-level computing backends and cutting edge algorithm implementations to solve large-scale Machine Learning problems (yet) on single machines.

-------------------------------------------------------------------------------

# Project about DevOps

## Code Repository

- [Git](http://www.git-scm.com/): Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
- [Gitlab](https://about.gitlab.com/): Open source git server
- [bonobo git server](https://bonobogitserver.com/): Simple git server for Windows. Set up your own self hosted git server on IIS for Windows. Manage users and have full control over your repositories with a nice user friendly graphical interface.
- [gitosis](https://github.com/res0nat0r/gitosis): software for hosting git repositories
- [gitolite](https://github.com/sitaramc/gitolite): Hosting git repositories -- Gitolite allows you to setup git hosting on a central server, with very fine-grained access control and many (many!) more powerful features.

## Code Analysis and Metrics

- [StyleCop](https://stylecop.codeplex.com/) - StyleCop analyzes C# source code to enforce a set of style and consistency rules
- [FoxCop](https://msdn.microsoft.com/en-us/library/bb429476(v=vs.80).aspx) - FxCop is an application that analyzes managed code assemblies (code that targets the .NET Framework common language runtime) and reports information about the assemblies, such as possible design, localization, performance, and security improvements.
- [SonarQube](http://www.sonarqube.org/): SonarQube is an open platform to manage code quality. As such, it covers the 7 axes of code quality:
- [OpenCover](https://github.com/OpenCover/opencover): A code coverage tool for .NET 2 and above, support for 32 and 64 processes with both branch and sequence points; roots proudly based in PartCover

## Documentation

- [Sandcastle](http://shfb.codeplex.com/) - Sandcastle Help File Builder similar to NDoc
- [SharpDox](https://github.com/Geaz/sharpDox) - A c# documentation tool

## Build Automation

- [Psake](https://github.com/psake/psake) - .NET-based build automation tool written in PowerShell
- [Invoke-Build](https://github.com/nightroman/Invoke-Build) - PowerShell build and test automation tool inspired by Psake.
- [MSBuild](https://github.com/Microsoft/msbuild) - The Microsoft Build Engine (MSBuild) is the build platform for .NET and Visual Studio
- [Wixtoolset](http://wixtoolset.org/): The WiX toolset builds Windows installation packages from XML source code. The toolset integrates seamlessly into build processes.
- [gradle](http://gradle.org/): OPEN SOURCE BUILD AUTOMATION. Get started with: Java / JVM | Android | Native (C / C++) | Web and many more!

## Continuous Integration

- [CruiseControl.NET](http://www.cruisecontrolnet.org/) - an Automated Continuous Integration server, implemented using the .NET Framework
- [MyGet](http://www.myget.org/) - Continuous Integration and Deployment, Hosted Package Repository for NuGet, NPM, Bower and VSIX. [Free for OSS] [$]
- [Jenkins-CI](http://jenkins-ci.org/): An extensible open source continuous integration server
- [Go Continuous Delivery](http://www.go.cd/): Automate and streamline the build-test-release cycle for worry-free, continuous delivery of your product.
- [janky](https://github.com/github/janky): Continuous integration server built on top of Jenkins and Hubot

## Unit Testing

- [NUnit](https://github.com/nunit/nunit-framework)
- [xUnit](https://github.com/xunit/xunit) - xUnit.net is a free, open source, community-focused unit testing tool for the .NET Framework
- [SpecFlow](https://github.com/techtalk/SpecFlow/) - Binding business requirements to .Net code
- [AutoFixture](https://github.com/AutoFixture/AutoFixture) - AutoFixture is an open source framework for .NET designed to minimize the 'Arrange' phase of your unit tests
- [Moq](https://github.com/Moq/moq4) - The most popular and friendly mocking framework for .NET
- [Machine.Specifications](https://github.com/machine/machine.specifications) - Machine.Specifications (MSpec) is a context/specification framework that removes language noise and simplifies tests.
- [Rhino Mocks](https://github.com/ayende/rhino-mocks) - Dynamic Mocking Framework for .NET
- [Fluent Assertions](https://github.com/dennisdoomen/fluentassertions) - A set of .NET extension methods that allow you to more naturally specify the expected outcome of a TDD or BDD-style test
- [NSubstitute](http://nsubstitute.github.io/) - A friendly substitute for .NET mocking frameworks
- [NBuilder](https://github.com/garethdown44/nbuilder) - Rapid generation of test objects

## Database Testing

- [dbUnit](http://dbunit.sourceforge.net/intro.html): database unit testing
- [TSQLT](http://tsqlt.org/): tSQLt is a database unit testing framework for Microsoft SQL Server. tSQLt is compatible with SQL Server 2005 (service pack 2 required) and above on all editions.
- [DbFit](http://dbfit.github.io/dbfit/index.html): Test-driven database development. Write readable, easy-to-maintain unit and integration tests for your database code.

## Automated Acceptance Testing

- [fitnesse](http://www.fitnesse.org/FrontPage): The fully integrated standalone wiki and acceptance testing framework
- [Cumuber](https://cucumber.io/): Cucumber is a software tool that computer programmers use for testing other software. It runs automated acceptance tests written in a behavior-driven development (BDD) style.
- [SpecFlow](http://www.specflow.org/): SpecFlow aims at bridging the communication gap between domain experts and developers by binding business readable behavior specifications and examples to the underlying implementation.
- [Selenium](http://www.seleniumhq.org/): Selenium is a suite of tools to automate web browsers across many platforms.
- [ROBOT FRAMEWORK](http://robotframework.org/): Robot Framework is a generic test automation framework for acceptance testing and acceptance test-driven development (ATDD).

## Performance Testing

- [Gor](https://github.com/buger/gor): Gor is a simple http traffic replication tool written in Go. Its main goal is to replay traffic from production servers to staging and dev environments.
- [Web Bench](http://home.tiscali.cz:8080/~cz210552/webbench.html): Web Bench是一个简单的web或者web代理服务的基准测试工具。（它）使用fork()模拟多个客户端并且可以发起HTTP/0/9-HTTP/1.1的请求。这个基准测试不是非常符合实际情况，但是可以测试出你的HTTP服务是否可以处理多个客户同时访问而不会把你的机器弄挂掉。这个工具可以获得服务的两个指标：每分钟响应请求数量（pages/min）和每秒钟传输数据量（bytes/sec）。
- [Siege](https://www.joedog.org/siege-home/): Siege（英文意思是围攻）是一个压力测试和评测工具，设计用于WEB开发这评估应用在压力下的承受能力：可以根据配置对一个WEB站点进行多用户的并发访问，记录每个用户所有请求过程的相应时间，并在一定数量的并发访问下重复进行。 Siege 支持基本的认证，cookies， HTTP 和 HTTPS 协议。
- [ab - Apache HTTP server benchmarking tool](http://jmeter.apache.org/): ab命令会创建很多的并发访问线程，模拟多个访问者同时对某一URL地址进行访问。它的测试目标是基于URL的，因此，既可以用来测试Apache的负载压力，也可以测试nginx、lighthttp、tomcat、IIS等其它Web服务器的压力。ab命令对发出负载的计算机要求很低，既不会占用很高CPU，也不会占用很多内存，但却会给目标服务器造成巨大的负载，其原理类似CC攻击。
- [TCPCopy](https://github.com/session-replay-tools/tcpcopy): TCPCopy is a TCP stream replay tool to support real testing of Internet server applications.
- [Apache JMeter](http://jmeter.apache.org/): Apache JMeter是一个专门为运行和服务器装载测试而设计的、100％的纯Java桌面运行程序。原先它是为Web/HTTP测试而设计的，但是它已经扩展以支持各种各样的测试模块。它和用于HTTP和SQL数据库（使用JDBC）的模块一起运送。它可以用来测试静止资料库或者活动资料库中的服务器的运行情况，可以用来模拟对服务器或者网络系统加以重负荷以测试它的抵抗力，或者用来分析不同负荷类型下的所有运行情况。它也提供了一个可替换的界面用来定制数据显示，测试同步及测试的创建和执行。
- [Badboy](http://www.badboy.com.au/): Badboy is a powerful tool designed to aid in testing and development of complex dynamic applications. Badboy makes web testing and development easier with dozens of features including a simple yet comprehensive capture/replay interface, powerful load testing support, detailed reports, graphs and much more!
- [Gatling](http://gatling.io/): Gatling is an open-source load testing framework based on Scala, Akka and Netty
- [West Wind Websurge](http://websurge.west-wind.com/): We believe that testing HTTP requests and load testing a site should be easy - something that takes a few minutes to set up and then runs on a regular basis during the development process, so that you can monitor performance of your site while you are building it. To this end we built West Wind WebSurge with the developer and testers in mind to make it easy to create HTTP requests or entire sessions, and then easily play back either individual URLs for development response testing, or for full-on testing under heavy load. Sessions are stored in plain text files so that they can be easily stored with projects or shared via source control for all users to have access.

## System Monitor

- [Opserver](https://github.com/opserver/opserver): Opserver is a monitoring system by the team at Stack Exchange, home of Stack Overflow.
- [Zabbix](http://www.zabbix.com/): Zabbix is the ultimate enterprise-level software designed for real-time monitoring of millions of metrics collected from tens of thousands of servers, virtual machines and network devices.
- [Nagios](https://www.nagios.org/): Nagios Is The Industry Standard In IT Infrastructure Monitoring. Achieve instant awareness of IT infrastructure problems, so downtime doesn't adversely affect your business.

## Deployment

- [Unfold](https://github.com/thomasvm/unfold) - Powershell-based deployment solution for .net web applications

## User Behavior Collection & Analysis

- [Piwik - Open Analytics Platform](http://piwik.org/): Piwik is an open analytics platform currently used by individuals, companies and governments all over the world. With Piwik, your data will always be yours. Learn why Piwik is the right web analytics tool for you below.
- [Open Web Analytics](http://www.openwebanalytics.com/): Open Web Analytics (OWA) is open source web analytics software that you can use to track and analyze how people use your websites and applications. OWA is licensed under GPL and provides website owners and developers with easy ways to add web analytics to their sites using simple Javascript, PHP, or REST based APIs.
- [Snowplow - the event analytics platform](http://snowplowanalytics.com/): Have every single event, from your websites, mobile apps, desktop applications and server-side systems, stored in your own data warehouse and available to action in real-time.
- [tracking.js](http://trackingjs.com/): The tracking.js library brings different computer vision algorithms and techniques into the browser environment. By using modern HTML5 specifications, we enable you to do real-time color tracking, face detection and much more — all that with a lightweight core (~7 KB) and intuitive interface.

## Infrastructure Management

- [Apache Mesos](http://mesos.apache.org/): Apache Mesos abstracts CPU, memory, storage, and other compute resources away from machines (physical or virtual), enabling fault-tolerant and elastic distributed systems to easily be built and run effectively.

## Misc

- [Apache Flume](http://flume.apache.org/): Flume is a distributed, reliable, and available service for efficiently collecting, aggregating, and moving large amounts of log data. It has a simple and flexible architecture based on streaming data flows. It is robust and fault tolerant with tunable reliability mechanisms and many failover and recovery mechanisms. It uses a simple extensible data model that allows for online analytic application.
- [twill](http://twill.idyll.org/): a simple scripting language for Web browsing

-------------------------------------------------------------------------------

# Articles

## .NET Language & CLR

- 2010-04-03: [编程语言的发展趋势及未来方向(系列文章)](http://blog.zhaojie.me/2010/04/trends-and-future-directions-in-programming-languages-by-anders-1-history-and-trends.html)
- 2010-08-18: [C# 4动态编程新特性与DLR剖析](http://www.cnblogs.com/bitfan/archive/2010/08/18/1802769.html)
- 2014-12-04: [Introducing .NET Core](http://blogs.msdn.com/b/dotnet/archive/2014/12/04/introducing-net-core.aspx)
- 2015-07-12: [CLR 这些年有啥变化吗？](http://www.cnblogs.com/HQFZ/p/4638239.html)
- 2015-07-22: [.NET技术大系概览 （迄今为止最全的.NET技术栈）](http://www.cnblogs.com/unruledboy/p/NetStack.html)

Mono:  

- 2012-07-28: [国内 Mono 相关文章汇总](http://www.cnblogs.com/shanyou/archive/2012/07/28/2612919.html)

Misc:  

- 2009-03-25: [significant differences between the CLR and the JVM](http://stackoverflow.com/questions/682608/implementing-c-sharp-for-the-jvm)

## Web Development

- 2009-01-23: [Exploring Session in ASP.NET](http://www.codeproject.com/Articles/32545/Exploring-Session-in-ASP-Net)
- 2012-02-29: [What's New in ASP.NET 4.5 and Visual Studio 2012](http://www.asp.net/aspnet/overview/aspnet-and-visual-studio-2012/whats-new)
- 2012-04-15: [How to: Sample Session-State Store Provider](https://msdn.microsoft.com/en-us/library/vstudio/ms178589(v=vs.100).aspx)
- 2012-08-23: [Bundling and Minification](http://www.asp.net/mvc/overview/performance/bundling-and-minification)
- 2012-09-09: [Introducing ASP.NET FriendlyUrls - cleaner URLs, easier Routing, and Mobile Views for ASP.NET Web Forms](http://www.hanselman.com/blog/IntroducingASPNETFriendlyUrlsCleanerURLsEasierRoutingAndMobileViewsForASPNETWebForms.aspx)
- 2013-01-04: [选择HttpHandler还是HttpModule？](http://www.cnblogs.com/fish-li/archive/2013/01/04/2844908.html)
- 2013-05-27: [What is Katana and OWIN for ASP.NET?](http://www.techbubbles.com/aspnet/what-is-katana-and-owin-for-asp-net/)
- 2013-10-03: [ASP.NET Web API OWIN Self Host on Windows Azure](http://weblogs.asp.net/shijuvarghese/asp-net-web-api-owin-self-host-on-windows-azure?utm_source=tuicool)
- 2014-05-18: [The Future of .NET on the Server: ASP.NET vNext content and videos from TechEd 2014](http://www.hanselman.com/blog/TheFutureOfNETOnTheServerASPNETVNextContentAndVideosFromTechEd2014.aspx)
- 2015-02-23: [Introducing ASP.NET 5 - scottgu](https://weblogs.asp.net/scottgu/introducing-asp-net-5)
- 2015-05-20: [How to Use Azure Redis Cache](https://azure.microsoft.com/en-us/documentation/articles/cache-dotnet-how-to-use-azure-redis-cache/)


## Distributed Architecture

### Common

- 2013-03-31: [分布式系统编程，你到哪一级了？](http://blog.jobbole.com/20304/)
- 2014-11-20: [How to start learning high scalability](http://leandromoreira.com.br/2014/11/20/how-to-start-to-learn-high-scalability/)
- 2015-06-02: [系统架构领域的一些学习材料](http://www.wtoutiao.com/p/f04hok.html)

Message Exchange Format:

- 2011-08-01: [Protocol Buffers, Avro, Thrift & MessagePack](https://www.igvita.com/2011/08/01/protocol-buffers-avro-thrift-messagepack/)
- 2013-05-16: [PB vs Thrift vs Avro](http://www.cnblogs.com/fxjwind/archive/2013/05/16/3082219.html)

### Load Balance

- 2013-08-08: [系列文章: Writing a reverse proxy/loadbalancer from the ground up in C](http://www.gilesthomas.com/2013/08/writing-a-reverse-proxyloadbalancer-from-the-ground-up-in-c-part-0/)
- 2014-07-21: [（总结）Nginx/LVS/HAProxy负载均衡软件的优缺点详解](http://www.ha97.com/5646.html)
- 2015-07-10: [Azure Load Balancer Overview](https://azure.microsoft.com/zh-cn/documentation/articles/load-balancer-overview/)
- 2015-07-15: [使用IIS Application Request Routing](http://www.iis.net/downloads/microsoft/application-request-routing)

### Service Bus & Message Queue

- [ESB Content On InfoQ](http://www.infoq.com/esb)
- 2006-10-23: [The Role of the Enterprise Service Bus](http://www.infoq.com/presentations/Enterprise-Service-Bus)
- 2009-06-18: [nServiceBus, Rhino Service Bus, MassTransit - Videos, Demos, Learning Resources](http://stackoverflow.com/questions/1012289/nservicebus-rhino-service-bus-masstransit-videos-demos-learning-resources)
- 2013-03-23: [企业服务总线Enterprise service bus介绍](http://www.cnblogs.com/wintersun/archive/2013/03/23/2977875.html)

Azure Service Bus:

- 2015-06-09: [Azure Service Bus fundamentals](https://azure.microsoft.com/en-us/documentation/articles/fundamentals-service-bus-hybrid-solutions/)
- 2015-05-21: [Azure Queues and Service Bus queues - compared and contrasted](https://azure.microsoft.com/en-us/documentation/articles/service-bus-azure-and-service-bus-queues-compared-contrasted/)

MassTransit

//todo: add article from http://blog.phatboyg.com/, http://codebetter.com/drusellers/

### Distributed Computing

- 2013-12-11: [分布式应用框架Akka快速入门](http://blog.csdn.net/jmppok/article/details/17264495)

### Distributed File System

- [分布式文件系统研究（Distributed File System Study）](http://www.docin.com/p-84299387.html)
- [7种分布式文件系统介绍](http://wenku.baidu.com/view/55a6745e3b3567ec102d8aea.html)

### Search

- [Apache Solr vs ElasticSearch](http://solr-vs-elasticsearch.com/)

### Recommender System

- [Recommender systems, Part 1: Introduction to approaches and algorithms](http://www.ibm.com/developerworks/library/os-recommender1/index.html)
- [Recommender systems, Part 2: Introducing open source engines](http://www.ibm.com/developerworks/library/os-recommender2/index.html)
- [TOP 10开源的推荐系统简介](http://ibillxia.github.io/blog/2014/03/10/top-10-open-source-recommendation-systems/)
- [ 推荐系统开源软件列表汇总和点评](http://blog.csdn.net/cserchen/article/details/14231153)

### NoSQL Database

- [TokuMX使用小计](http://blogread.cn/it/article/6959)

### Distributed Realtime Computation System

- 2013-12-16: [The Log: What every software engineer should know about real-time data's unifying abstraction](http://engineering.linkedin.com/distributed-systems/log-what-every-software-engineer-should-know-about-real-time-datas-unifying)
- 2015-03-22: [Where do Apache Samza and Apache Storm differ in their use cases?](http://stackoverflow.com/questions/29111549/where-do-apache-samza-and-apache-storm-differ-in-their-use-cases)
- 2015-06-30: [浅谈《【原创】深度分析Twitter Heron》](http://maosongfu.roughdraft.io/c3aeb1bb5eb7b39fcdc5-)
- 2015-07-16: [学习笔记：The Log（我所读过的最好的一篇分布式技术文章）](http://www.cnblogs.com/foreach-break/p/notes_about_distributed_system_and_The_log.html)


## DevOps

### Performance & Monitor

- 2011-08-30: [IoC Container Benchmark - Performance comparison](http://www.palmmedia.de/Blog/2011/8/30/ioc-container-benchmark-performance-comparison)
- 2013-01-06: [Replace JSON.NET with ServiceStack.Text in ASP.NET Web API](http://www.strathweb.com/2013/01/replace-json-net-with-servicestack-text-in-asp-net-web-api/)
- 2013-02-24: [ASP.NET Web API and Protocol Buffers](http://www.strathweb.com/2013/02/asp-net-web-api-and-protocol-buffers/)
- 2013-11-09: [采访ServiceStack的项目领导Demis Bellot——第1部分](http://www.infoq.com/cn/articles/interview-servicestack)
- 2013-11-21: [采访ServiceStack的项目领导Demis Bellot——第2部分](http://www.infoq.com/cn/articles/interview-servicestack-2)
- 2014-07-16: [8 ways to improve ASP.NET Web API performance](http://blog.developers.ba/8-ways-improve-asp-net-web-api-performance/)
- 2015-03-29: [池化.NET内存流以解决大内存堆分配问题](http://www.infoq.com/cn/news/2015/03/Memory-Stream)
- 2015-07-06: [Stack Overflow通过关注性能，实现单块应用架构的扩展能力](http://www.infoq.com/cn/news/2015/07/scaling-stack-overflow)
- 2015-07-16: [使用 West Wind WebSurge 对 ASP.NET Web API 服务进行压力测试](http://www.cnblogs.com/shanyou/p/4651084.html)
- 2015-07-23: [.NET 4.6中的性能改进](http://www.infoq.com/cn/news/2015/07/Net-46-Performance)

### Monitor

- 2013-12-12: [初识Opserver，StackExchange的监控解决方案](http://www.infoq.com/cn/news/2013/12/first_look_at_opserver)
- 2015-04-26: [Get started with Visual Studio Application Insights](https://azure.microsoft.com/en-us/documentation/articles/app-insights-get-started/?rnd=1)

### Test

- 2011-01-11: [行为驱动开发之一，推广篇](http://www.cnblogs.com/jarodzz/archive/2011/03/16/1986551.html)
- 2011-03-21: [行为驱动开发之二，实施篇](http://www.cnblogs.com/jarodzz/archive/2011/03/21/1989890.html)
- 2011-03-28: [行为驱动开发之三，从测试驱动开发中来](http://www.cnblogs.com/jarodzz/archive/2011/03/28/1997366.html)
- 2011-03-28: [行为驱动开发之三，从测试驱动开发中来](http://www.cnblogs.com/jarodzz/archive/2011/03/28/1997366.html)
- 2011-09-02: [行为驱动开发之四，为自动化测试（运行Cucumber）提速](http://www.cnblogs.com/jarodzz/archive/2011/09/02/bdd4.html)
- 2011-10-02: [行为驱动开发之五，迅雷模式与笨蛋](http://www.cnblogs.com/jarodzz/archive/2011/10/03/2198620.html)
- 2012-07-02: [Cucumber入门1 - 传统流程下的使用](http://www.cnblogs.com/jarodzz/archive/2012/07/02/2573014.html)
- 2012-07-26: [Cucumber入门2 - 啥是BDD？](http://www.cnblogs.com/jarodzz/archive/2012/07/26/2610617.html)
- 2014-05-09: [自动化单元测试实践之路](http://www.infoq.com/cn/articles/road-of-automated-unit-testing-practices)
- 2014-05-11: [几个性能测试工具](http://www.cnblogs.com/EthanCai/p/3721656.html)
- 2015-07-11: [Web 应用性能和压力测试工具 Gor](http://mp.weixin.qq.com/s?__biz=MjM5NjQ4MjYwMQ==&mid=208024569&idx=4&sn=168cf756825bc205866d541a2bdd3878&scene=1&from=groupmessage&isappinstalled=0#rd)



-------------------------------------------------------------------------------

# References

- [Patterns & Practices](https://msdn.microsoft.com/en-us/library/ff921345.aspx)
- [Awesome dotNET](https://github.com/quozd/awesome-dotnet)
- [Open Source Testing](http://www.opensourcetesting.org/)
- [NoSQL Database](http://nosql-database.org/)
- [amplab - UC BERKELEY](https://amplab.cs.berkeley.edu/)
- [A Complete List of .NET Open Source Developer Projects](http://scottge.net/2015/07/08/a-complete-list-of-net-open-source-developer-projects/)