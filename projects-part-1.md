<!-- MDTOC maxdepth:6 firsth1:1 numbering:0 flatten:0 bullets:1 updateOnSave:1 -->

- [Projects about Normal Software Development](#projects-about-normal-software-development)
   - [Compiler](#compiler)
   - [Language Converter](#language-converter)
   - [Interpreter](#interpreter)
   - [Debugger](#debugger)
   - [Analyzer](#analyzer)
   - [Profiling](#profiling)
   - [Assembly Manipulation](#assembly-manipulation)
   - [Web Servers & Application Servers](#web-servers-application-servers)
   - [Application Frameworks](#application-frameworks)
   - [Template Engine](#template-engine)
   - [GUI Framework](#gui-framework)
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
   - [File](#file)
   - [Image Processing](#image-processing)
   - [Audio & Video](#audio-video)
   - [Computer Vision](#computer-vision)
   - [Authentication & Authorization](#authentication-authorization)
   - [Mail](#mail)
   - [State Machine](#state-machine)
   - [Tools](#tools)
   - [.NET Interoperability](#net-interoperability)
   - [Windows Services](#windows-services)
   - [Misc Libraries](#misc-libraries)

<!-- /MDTOC -->

# Projects about Normal Software Development

## Compiler

- [LLVM](http://www.llvm.org/): The LLVM Project is a collection of modular and reusable compiler and toolchain technologies. Despite its name, LLVM has little to do with traditional virtual machines. The name "LLVM" itself is not an acronym; it is the full name of the project.
- [.NET Core](http://dotnet.github.io/core/): A general purpose managed framework
- [.NET: Mono](http://www.mono-project.com/): Cross platform, open source .NET framework
- [.NET: Roslyn](https://github.com/dotnet/roslyn): The .NET Compiler Platform ("Roslyn") provides open-source C# and Visual Basic compilers with rich code analysis APIs.
- [Java: OpenJDK](http://openjdk.java.net/): open-source implementation of the Java Platform, Standard Edition
- [Java: Oracle JDK](http://www.oracle.com/technetwork/java/javase/overview/index.html): N/A
- [Java: Eclipse OpenJ9](http://www.eclipse.org/openj9/): IBM已经开源自己的JDK作为Eclipse OpenJ9

## Language Converter

- [Golang: gopherjs](https://github.com/gopherjs/gopherjs): GopherJS compiles Go code (golang.org) to pure JavaScript code. Its main purpose is to give you the opportunity to write front-end code in Go which will still run in all browsers.

## Interpreter

- [Golang: Otto](https://github.com/robertkrimen/otto): A JavaScript interpreter in Go (golang)
- [C++: V8 JavaScript Engine](https://github.com/v8/v8): Google's open source JavaScript engine.

## Debugger

- [GDB](https://www.gnu.org/software/gdb/): The GNU Project Debugger
- [gdbgui](https://github.com/cs01/gdbgui): A modern, browser-based frontend to gdb (gnu debugger). Add breakpoints, view stack traces, and more in C, C++, Go, and Rust. Simply run gdbgui from the terminal and a new tab will open in your browser.
- [rr](https://github.com/mozilla/rr): rr is a lightweight tool for recording and replaying execution of applications (trees of processes and threads). rr aspires to be your primary C/C++ debugging tool for Linux, replacing — well, enhancing — gdb. You record a failure once, then debug the recording, deterministically, as many times as you want. The same execution is replayed every time.
- [LLDB Debugger](http://lldb.llvm.org/): LLDB is a next generation, high-performance debugger. It is built as a set of reusable components which highly leverage existing libraries in the larger LLVM Project, such as the Clang expression parser and LLVM disassembler. LLDB is the default debugger in Xcode on Mac OS X and supports debugging C, Objective-C and C++ on the desktop and iOS devices and simulator.
- [Golang: Delve](https://github.com/derekparker/delve/): Delve is a debugger for the Go programming language.

## Analyzer

- [Golang: goviz](https://github.com/hirokidaichi/goviz): a visualization tool for golang project dependency
- [Golang: godepq](https://github.com/google/godepq): A utility for inspecting go import trees

## Profiling

- [Golang: go-torch](https://github.com/uber/go-torch): Stochastic flame graph profiler for Go programs

## Assembly Manipulation

- [.NET: Fody](https://github.com/Fody/Fody) - Extensible tool for weaving .net assemblies
- [.NET: Mono.Cecil](https://github.com/jbevain/cecil) - Cecil is a library to generate and inspect programs and libraries in the ECMA CIL form.

## Web Servers & Application Servers

- [Nginx](http://wiki.nginx.org/Main): a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
    - [OpenResty](http://openresty.org/): OpenResty (aka. ngx_openresty) is a full-fledged web application server by bundling the standard Nginx core, lots of 3rd-party Nginx modules, as well as most of their external dependencies.
    - [Tengine](http://tengine.taobao.org/): Tengine是由淘宝网发起的Web服务器项目。它在Nginx的基础上，针对大访问量网站的需求，添加了很多高级功能和特性。Tengine的性能和稳定性已经在大型的网站如淘宝网，天猫商城等得到了很好的检验。它的最终目标是打造一个高效、稳定、安全、易用的Web平台。
    - [VeryNginx](https://github.com/alexazhou/VeryNginx): 功能强大并且拥有对人类友好界面的Nginx, 提供防火墙，自定义行为和统计功能
- [lightttpd](http://www.lighttpd.net/): Security, speed, compliance, and flexibility -- all of these describe lighttpd (pron. lighty) which is rapidly redefining efficiency of a webserver; as it is designed and optimized for high performance environments. With a small memory footprint compared to other web-servers, effective management of the cpu-load, and advanced feature set (FastCGI, SCGI, Auth, Output-Compression, URL-Rewriting and many more) lighttpd is the perfect solution for every server that is suffering load problems. And best of all it's Open Source licensed under the revised BSD license.
- [.NET: KestrelHttpServer](https://github.com/aspnet/KestrelHttpServer): A cross platform web server for ASP.NET Core.
- [Java: Tomcat](http://tomcat.apache.org/): The Apache Tomcat® software is an open source implementation of the Java Servlet, JavaServer Pages, Java Expression Language and Java WebSocket technologies. The Java Servlet, JavaServer Pages, Java Expression Language and Java WebSocket specifications are developed under the Java Community Process.
- [Java: Jetty](http://www.eclipse.org/jetty/): Jetty provides a Web server and javax.servlet container, plus support for HTTP/2, WebSocket, OSGi, JMX, JNDI, JAAS and many other integrations. These components are open source and available for commercial use and distribution.

## Application Frameworks

Application Framework预备知识：

- [Wiki2 - Web framework](https://wiki2.org/en/Web_framework)
- [谁是最快的Go Web框架](http://colobu.com/2016/04/06/the-fastest-golang-web-framework/)
- [Github Showcases - Web application frameworks](https://github.com/showcases/web-application-frameworks?s=stars)
- [15 Important Considerations for Choosing A Web Dev Framework](https://code.tutsplus.com/tutorials/15-important-considerations-for-choosing-a-web-dev-framework--net-8035)


Application Frameworks:

- [Go: Beego](http://beego.me/): 一个使用 Go 的思维来帮助您构建并开发 Go 应用程序的开源框架
- [Go: Gin](https://github.com/gin-gonic/gin): Gin is a web framework written in Golang. It features a martini-like API with much better performance, up to 40 times faster thanks to httprouter. If you need performance and good productivity, you will love Gin.
- [Go: Iris](https://github.com/kataras/iris): The fastest web framework for Go in (THIS) earth
- [Go: revel](http://revel.github.io/): A high-productivity web framework for the Go language.
- [Nodejs: Expressjs](http://expressjs.com/): Fast, unopinionated, minimalist web framework for Node.js
- [Nodejs: Koa](https://github.com/koajs/koa): Expressive middleware for node.js using ES2017 async functions
- [Java: Spring Framework](http://spring.io/projects): The Spring Framework provides a comprehensive programming and configuration model for modern Java-based enterprise applications - on any kind of deployment platform.
	- [Java: jHipster](https://jhipster.github.io/): Open Source application generator for creating Spring Boot + AngularJS projects in seconds
- [Java: Akka](http://akka.io/): Akka is a toolkit and runtime for building highly concurrent, distributed, and resilient message-driven applications on the JVM. The power of Akka is also available on the .NET Framework and Mono via the Akka.NET project.
- [Java: Vert.x](http://vertx.io): Vert.x is a tool-kit for building reactive applications on the JVM.
- [Java: Netty](http://netty.io/): Netty is a NIO client server framework which enables quick and easy development of network applications such as protocol servers and clients. It greatly simplifies and streamlines network programming such as TCP and UDP socket server.
	- [Java: Mina](https://mina.apache.org/mina-project/index.html): Apache MINA is a network application framework which helps users develop high performance and high scalability network applications easily. It provides an abstract ·event-driven · asynchronous API over various transports such as TCP/IP and UDP/IP via Java NIO.
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

参考：

- [goTemplateBenchmark](https://github.com/SlinSo/goTemplateBenchmark)

## GUI Framework

- [Node: NW.js](https://github.com/nwjs/nw.js): Call all Node.js modules directly from DOM/WebWorker and enable a new way of writing applications with all Web technologies.
- [Node: Electron](https://electron.atom.io/): Build cross platform desktop apps with JavaScript, HTML, and CSS
	- [Node: Photon](https://github.com/connors/photon): The fastest way to build beautiful Electron apps using simple HTML and CSS
- [Java: Swing](https://wiki2.org/en/Java_Swing): Swing is a GUI widget toolkit for Java.
- [Java: SWT - Standard Widget Toolkit](https://eclipse.org/swt/): SWT is an open source widget toolkit for Java designed to provide efficient, portable access to the user-interface facilities of the operating systems on which it is implemented.
- [C++: QT](https://www.qt.io/): A complete cross-platform software framework with ready-made UI elements, C++ libraries, and a complete integrated development environment with tools for everything you need to develop software for any project.
- [C++: wxWidgets](https://www.wxwidgets.org/): wxWidgets is a C++ library that lets developers create applications for Windows, Mac OS X, Linux and other platforms with a single code base.
- [C/C++: GTK+](https://www.gtk.org/): GTK+, or the GIMP Toolkit, is a multi-platform toolkit for creating graphical user interfaces. Offering a complete set of widgets, GTK+ is suitable for projects ranging from small one-off tools to complete application suites.

References:

- [Intellij Community](https://github.com/JetBrains/intellij-community): which use Java Swing to implement it's GUI

## Asynchronous Programming Framework

- [ReactiveX](http://reactivex.io/): An API for asynchronous programming with observable streams
  - [Java: RxJava](https://github.com/ReactiveX/RxJava)
  - [Go: RxGo](https://github.com/ReactiveX/RxGo)
  - [JavaScript: RxJS](https://github.com/Reactive-Extensions/RxJS)
  - [C#: Rx.NET](https://github.com/Reactive-Extensions/Rx.NET)
  - C#(Unity): UniRx
  - Scala: RxScala
  - Clojure: RxClojure
  - C++: RxCpp
  - Lua: RxLua
  - Ruby: Rx.rb
  - Python: RxPY
  - Groovy: RxGroovy
  - JRuby: RxJRuby
  - Kotlin: RxKotlin
  - Swift: RxSwift
  - PHP: RxPHP
  - Elixir: reaxive
  - Dart: RxDart

## Web Socket

- [Go: Web Socket](https://github.com/gorilla/websocket): A WebSocket implementation for Go.
- [Go: centrifugo](https://github.com/centrifugal/centrifugo): Real-time messaging (Websockets or SockJS) server in Go
- [.NET: SignalR](https://github.com/SignalR/SignalR): Library for ASP.NET developers that makes it incredibly simple to add real-time web functionality to your applications
- [.NET: Fleck](https://github.com/statianzo/Fleck) - Fleck is a WebSocket server implementation in C#. Branched from the Nugget project
- [.NET: Websocket-Sharp](https://github.com/sta/websocket-sharp) - A C# implementation of the WebSocket protocol client and server
- [.NET: WebSocket4NET](https://websocket4net.codeplex.com/) - WebSocket client for .NET 2.0+, Xamarin, Mono, Silverlight, Windows Phone, & WinRT
- [.NET: XSockets](https://xsockets.net/) - Provides a great set of tools for you to build real-time applications on the Microsoft.NET plattform and much more
- [.NET: WampSharp](https://github.com/Code-Sharp/WampSharp) - A C# implementation of [The Web Application Messaging Protocol](http://wamp-proto.org/) - a protocol that provides messaging patterns of Remote Procedure Calls and Publish/Subscribe over WebSockets.

## Network

- [C++: Mars](https://github.com/Tencent/mars): Mars is a cross-platform network component developed by WeChat.
- [Go: kcptun](https://github.com/xtaci/kcptun): an extremely simple & fast udp tunnel based on kcp protocol
	- [Go: kcp-go](https://github.com/xtaci/kcp-go): A full-featured reliable UDP communication library
- [Go: goflyway](https://github.com/coyove/goflyway): HTTP tunnel in Go
- [Go: gorequest](https://github.com/parnurzeal/gorequest): Simplified HTTP client ( inspired by nodejs SuperAgent )
- [GO: DNS library](https://github.com/miekg/dns): DNS library in Go
- [Go: fasthttp](https://github.com/valyala/fasthttp): Fast HTTP package for Go. Tuned for high performance. Zero memory allocations in hot paths. Up to 10x faster than net/http.
- [Go: link](https://github.com/funny/link): Go语言网络层脚手架
- [Go: tus](http://www.oschina.net/p/tus): 一个开放的协议实现了客户端和服务器之间可恢复的文件上传协议
- [Go: sleuth](https://github.com/ursiform/sleuth): sleuth is a Go library that provides master-less peer-to-peer autodiscovery and RPC between HTTP services that reside on the same network. It works with minimal configuration and provides a mechanism to join a local network both as a client that offers no services and as any service that speaks HTTP. Its primary use case is for microservices on the same network that make calls to one another.
- [.NET: RestSharper](http://restsharp.org/): Simple REST and HTTP API Client for .NET
- [.NET: Fracture](https://github.com/fractureio/fracture): A high-performance socket I/O message pipeline library.
- [.NET: SuperSocket](http://www.supersocket.net/): SuperSocket 是一个轻量级, 跨平台而且可扩展的 .Net/Mono Socket 服务器程序框架。你无须了解如何使用 Socket, 如何维护 Socket 连接和 Socket 如何工作，但是你却可以使用 SuperSocket 很容易的开发出一款 Socket 服务器端软件，例如游戏服务器，GPS 服务器, 工业控制服务和数据采集服务器等等。

## Thread & Coroutine

- [C++: Libco](https://github.com/Tencent/libco): ibco是微信后台大规模使用的c/c++协程库，2013年至今稳定运行在微信后台的数万台机器上。libco通过仅有的几个函数接口 co_create/co_resume/co_yield 再配合 co_poll，可以支持同步或者异步的写法，如线程库一样轻松。同时库里面提供了socket族函数的hook，使得后台逻辑服务几乎不用修改逻辑代码就可以完成异步化改造。
- [C: libuv](https://github.com/libuv/libuv): Cross-platform asynchronous I/O
- [C: libev](https://github.com/enki/libev)
- [C: libevent](http://libevent.org/)
- [Rust: mio](https://github.com/carllerche/mio): Metal IO library for Rust

学习资料：

- [libuv 初窥](https://blog.codingnow.com/2012/01/libuv.html)
- [libuv中文教程](http://luohaha.github.io/Chinese-uvbook/index.html)：翻译自[An Introduction to libuv](http://nikhilm.github.io/uvbook/)
- [使用 libevent 和 libev 提高网络应用性能](https://www.ibm.com/developerworks/cn/aix/library/au-libev/index.html)
- [The C10K problem](http://www.kegel.com/c10k.html)

## IoC

- [Golang: facebookgo/inject](https://github.com/facebookgo/inject): Package inject provides a reflect based injector.
- [.NET: Castle Windsor](https://github.com/castleproject/Windsor) - Castle Windsor is best of breed, mature Inversion of Control container available for .NET and Silverlight
- [.NET: Unity](https://unity.codeplex.com/) - Lightweight extensible dependency injection container with support for constructor, property, and method call injection
- [.NET: Autofac](https://github.com/autofac/Autofac) - An addictive .NET IoC container
- [.NET: Ninject](https://github.com/ninject/ninject) - The ninja of .net dependency injectors
- [.NET: StructureMap](https://structuremap.github.io/) - The original IoC/DI Container for .Net
- [.NET: Spring.Net](https://github.com/spring-projects/spring-net) - Spring.NET is an open source application framework that makes building  enterprise .NET applications easier
- [.NET: LightInject](https://github.com/seesharper/LightInject) - A ultra lightweight IoC container
- [.NET: TinyIoC](https://github.com/grumpydev/TinyIoC) - Single-file, easy and cross-platform IoC container

## Logging

- [Go: zap](https://github.com/uber-go/zap): Fast, structured, leveled logging in Go
- [Go: logrus](https://github.com/Sirupsen/logrus): Structured, pluggable logging for Go.
- [Go: Apex/log](https://github.com/apex/log): Structured logging package for Go.
- [Go: stack](https://github.com/facebookgo/stack): provides utilities to capture and pass around stack traces.
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

- Golang
	- Database Drivers
		- [Golang: Go-MySQL-Driver](https://github.com/go-sql-driver/mysql): Go-MySQL-Driver is a lightweight and fast MySQL-Driver for Go's (golang) database/sql package
		- [Golang: pg](https://github.com/lib/pq): A pure Go postgres driver for Go's database/sql package
		- [Golang: sqlite](https://github.com/mattn/go-sqlite3): sqlite3 driver for go that using database/sql
		- [Golang: SQL Server](https://github.com/denisenkom/go-mssqldb): Microsoft SQL server driver written in go language
	- ORM
		- [Golang: gorm](https://github.com/jinzhu/gorm): The fantastic ORM library for Golang, aims to be developer friendly
		- [Golang: xorm](https://github.com/go-xorm/xorm): Simple and Powerful ORM for Go, support mysql/sqlite3/postgres/mssql/oracle/tidb/ql
		- [Golang: gorp](https://github.com/go-gorp/gorp): Go Relational Persistence - an ORM-ish library for Go
		- [Golang: go-pg](https://github.com/go-pg/pg): PostgreSQL ORM for Golang with focus on PostgreSQL features and performance
		- [Golang: Reform](https://github.com/go-reform/reform): A better ORM for Go, based on non-empty interfaces and code generation.
	- Tools
		- [Golang: sqlboiler](https://github.com/vattle/sqlboiler): SQLBoiler is a tool to generate a Go ORM tailored to your database schema.
		- [Golang: sql-migrate](https://github.com/rubenv/sql-migrate): SQL schema migration tool for Go
- Java
	- [Java: p6spy](https://github.com/p6spy/p6spy): P6Spy is a framework that enables database data to be seamlessly intercepted and logged with no code changes to the application. with no code changes to the application.
	- [Java: druid](https://github.com/alibaba/druid): 为监控而生的数据库连接池！
- .NET Framework
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

- [Go: go-simplejson](https://github.com/bitly/go-simplejson): a Go package to interact with arbitrary JSON
- [Go: Jason](https://github.com/antonholmquist/jason): Easy-to-use JSON Library for Go
- [Go: jsonpath](https://github.com/yalp/jsonpath): a (partial) implementation in Go based on [Stefan Goener JSON Path](http://goessner.net/articles/JsonPath/)
- [Go: gojsonschema](https://github.com/xeipuuv/gojsonschema): An implementation of JSON Schema, based on IETF's draft v4 - Go language
- [Go: gojsondiff](https://github.com/yudai/gojsondiff/): Go JSON Diff
- [Java: fastjson](https://github.com/alibaba/fastjson): A fast JSON parser/generator for Java
- [.NET: Jil](https://github.com/kevin-montrose/Jil): Fast .NET JSON (De)Serializer, Built On Sigil
- [.NET: ServiceStack.Text](https://github.com/ServiceStack/ServiceStack.Text): .NET's fastest JSON, JSV and CSV Text Serializers
- [.NET: Json.net](http://www.newtonsoft.com/json): Popular high-performance JSON framework for .NET
- [.NET: fastjson](https://fastjson.codeplex.com/): Smallest, fastest polymorphic JSON serializer

## Command Line

- [Go: viper](https://github.com/spf13/viper): Go configuration with fangs
- [Go: go-flags](https://github.com/jessevdk/go-flags): go command line option parser
- [Go: kingpin](https://github.com/alecthomas/kingpin): A Go (golang) command line and flag parser
- [.NET: Command Line Parser](https://github.com/gsscoder/commandline) - The Command Line Parser Library offers to CLR applications a clean and concise API for manipulating command line arguments and related tasks
- [.NET: Fluent Command Line Parser](https://github.com/fclp/fluent-command-line-parser) - A simple, strongly typed .NET C# command line parser library using a fluent easy to use interface
- [.NET: Power Args](https://github.com/adamabdelhamed/PowerArgs) - PowerArgs converts command line arguments into .NET objects that are easy to program against. It also provides a ton of optional capabilities such as argument validation, auto generated usage, tab completion, and plenty of extensibility

## Math

- [.NET: Math.NET](https://www.mathdotnet.com/)
	- [Math.NET Numerics: numerical computing](http://numerics.mathdotnet.com/): Math.NET Numerics aims to provide methods and algorithms for numerical computations in science, engineering and every day use. Covered topics include special functions, linear algebra, probability models, random numbers, interpolation, integration, regression, optimization problems and more.
	- [Math.NET Symbolics: computer algebra](http://symbolics.mathdotnet.com/): Math.NET Symbolics is a basic open source computer algebra library for .Net and Mono written in F#.
	- [Math.NET Filtering: signal processing](http://filtering.mathdotnet.com/): Filtering aims to provide a toolkit for digital signal processing, offering an infrastructure for digital filter design, applying those filters to data streams using data converters, as well as digital signal generators.
	- [Math.NET Spatial](http://spatial.mathdotnet.com/): Math.NET Spatial is aiming to become a geometry library for .Net and Mono.

## File

- [Go: fsnotify](https://github.com/fsnotify/fsnotify): File system notifications for Go.
- [Go: restic](https://github.com/restic/restic): restic is a backup program that is fast, efficient and secure.
- [Go: syncthing](https://github.com/syncthing/syncthing): Open Source Continuous File Synchronization
- [Go: go-ini](https://github.com/go-ini/ini): Package ini provides INI file read and write functionality in Go.
- [Go: xlsx](https://github.com/tealeg/xlsx): Google Go (golang) library for reading and writing XLSX files.

## Image Processing

- [Go: ln](https://github.com/fogleman/ln): ln is a vector-based 3D renderer written in Go. It is used to produce 2D vector graphics (think SVGs) depicting 3D scenes. The output of an OpenGL pipeline is a rastered image. The output of ln is a set of 2D vector paths.
- [C: ImageMagick](http://www.imagemagick.org): ImageMagick® is a software suite to create, edit, compose, or convert bitmap images. It can read and write images in a variety of formats (over 200) including PNG, JPEG, JPEG-2000, GIF, TIFF, DPX, EXR, WebP, Postscript, PDF, and SVG. Use ImageMagick to resize, flip, mirror, rotate, distort, shear and transform images, adjust image colors, apply various special effects, or draw text, lines, polygons, ellipses and Bézier curves.
- [C: GraphicsMagick](http://www.graphicsmagick.org): GraphicsMagick is the swiss army knife of image processing. Comprised of 267K physical lines (according to David A. Wheeler's SLOCCount) of source code in the base package (or 1,225K including 3rd party libraries) it provides a robust and efficient collection of tools and libraries which support reading, writing, and manipulating an image in over 88 major formats including important formats like DPX, GIF, JPEG, JPEG-2000, PNG, PDF, PNM, and TIFF.
- [.NET: ImageProcessor](http://imageprocessor.org/): ImageProcessor is a collection of lightweight libraries written in C# that allows you to manipulate images on-the-fly using .NET 4.5+
- [Hugin](http://sourceforge.net/projects/hugin): Panorama photo stitcher
- [Luminance HDR](http://sourceforge.net/projects/qtpfsgui): Complete solution for HDR photography
- [scikit-image](http://scikit-image.org/): scikit-image is a collection of algorithms for image processing. It is available free of charge and free of restriction.
- $[Pano2VR & Object2VR](http://ggnome.com/): software for interactive panoramas and object movies.

## Audio & Video

- [OpenGL](https://www.opengl.org/): The Industry Standard for High Performance Graphics
- [SoX](http://sox.sourceforge.net/): SoX is a cross-platform (Windows, Linux, MacOS X, etc.) command line utility that can convert various formats of computer audio files in to other formats. It can also apply various effects to these sound files, and, as an added bonus, SoX can play and record audio files on most platforms.
- [ffmpeg](https://www.ffmpeg.org/): A complete, cross-platform solution to record, convert and stream audio and video.
- [VLC media player](http://www.videolan.org/vlc/): VLC 是一款自由、开源的跨平台多媒体播放器及框架，可播放大多数多媒体文件，以及 DVD、音频 CD、VCD 及各类流媒体协议。

## Computer Vision

- [C: OpenCV](http://opencv.org/): OpenCV is released under a BSD license and hence it’s free for both academic and commercial use. It has C++, C, Python and Java interfaces and supports Windows, Linux, Mac OS, iOS and Android. OpenCV was designed for computational efficiency and with a strong focus on real-time applications. Written in optimized C/C++, the library can take advantage of multi-core processing. Enabled with OpenCL, it can take advantage of the hardware acceleration of the underlying heterogeneous compute platform. Adopted all around the world, OpenCV has more than 47 thousand people of user community and estimated number of downloads exceeding 9 million. Usage ranges from interactive art, to mines inspection, stitching maps on the web or through advanced robotics.
    - [Emgu CV](http://www.emgu.com/wiki/index.php/Emgu_CV): Emgu CV is a cross platform .Net wrapper to the OpenCV image processing library. Allowing OpenCV functions to be called from .NET compatible languages such as C#, VB, VC++, IronPython etc. The wrapper can be compiled by Visual Studio, Xamarin Studio and Unity, it can run on Windows, Linux, Mac OS X, iOS, Android and Windows Phone.
- [C: libccv](https://github.com/liuliu/ccv): C-based/Cached/Core Computer Vision Library, A Modern Computer Vision Library
- [.NET: AForge.NET](http://www.aforgenet.com/): AForge.NET is a C# framework designed for developers and researchers in the fields of Computer Vision and Artificial Intelligence - image processing, neural networks, genetic algorithms, machine learning, robotics, etc.

## Authentication & Authorization

- [Go: captcha](https://github.com/jianxinio/captcha): Golang实现的验证码服务
- [Go: Go OTP](https://github.com/hgfischer/go-otp): Package go-otp implements one-time-password generators used in 2-factor authentication systems like RSA-tokens. Currently this supports both HOTP (RFC-4226), TOTP (RFC-6238) and Base32 encoding (RFC-3548) for Google Authenticator compatibility
    - [Go-otpserver](https://github.com/skyjia/go-otpserver): A golang version OTP server.
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

## Tools

- [.NET: CS-Script](http://www.csscript.net/index.html): CS-Script is a CLR (Common Language Runtime) based scripting system which uses ECMA-compliant C# as a programming language. CS-Script currently targets Microsoft implementation of CLR (.NET 2.0/3.0/3.5/4.0/4.5) with full support on Mono.
- [.NET: Scriptcs](http://scriptcs.net/): Unleash your C# from Visual Studio.
- [.NET: dotPeek](https://www.jetbrains.com/decompiler/): Free .NET Decompiler and Assembly Browser
- [.NET: FastFileFinder](https://github.com/Wintellect/FastFileFinder): Find files and directory names FAST!
- [.NET: Rant2](https://github.com/TheBerkin/Rant): Rant is a language for procedurally generating text, written in C#. It combines a markup language with functional and imperative programming concepts to deliver a powerful, but easy-to-use tool for adding rich variations to your text. The ultimate goal of Rant is to augment your creativity with the boundless potential of randomness, helping you consider your next great idea as not just a static concept, but a seed for countless possibilities.

## .NET Interoperability

- [.NET: CppSharp](https://github.com/mono/CppSharp) - Tools to surface C++ APIs to C#
- [.NET: Sharpen](https://github.com/mono/sharpen) - Sharpen is an Eclipse plugin created by db4o that allows you to convert your Java project into C#
- [.NET: CXXI](https://github.com/mono/cxxi) - C++ interop framework

## Windows Services

- [.NET: Topshelf](http://topshelf-project.com/): Put Your Apps on the Topshelf

## Misc Libraries

- [C++: Boost](http://www.boost.org/)
- [C++: Abseil](https://abseil.io/)
- [Go: pointer](https://github.com/AlekSi/pointer): Go package pointer provides helpers to get pointers to values of build-in types.
- [Go: robpike.io/filter](https://godoc.org/robpike.io/filter): Package filter contains utility functions for filtering slices through the distributed application of a filter function.
- [Go: queue](https://github.com/eapache/queue):  not thread-safe queue
- [Go: safemap](https://github.com/pcrawfor/safemap): A golang channel based access object for shared use of a map of arbitrary objects
- [Go: i18n4go](https://github.com/maximilien/i18n4go): This is a general purpose internationalization (i18n) tooling for Go language (Golang) programs. It allows you to prepare Go language code for internationalization and localization (l10n).
- [.NET: AutoMapper](http://automapper.org/): a simple little library built to solve a deceptively complex problem - getting rid of code that mapped one object to another.
- [.NET: UrlRewriter](https://github.com/sethyates/urlrewriter): UrlRewriter.NET is an open-source, light-weight, highly configurable URL rewriting component for ASP.NET 1.1 – 4.0.
- [.NET: Fast Reflection Library](http://fastreflectionlib.codeplex.com/): FastReflectionLib provide the same as part of the refection features like executing method dynamically but give simple and faster implementations. It can be use as the foundation of reflection-based scenarios such as ORM framework.
- [.NET: FluentValidation](https://github.com/JeremySkinner/FluentValidation): A small validation library for .NET that uses a fluent interface and lambda expressions for building validation rules. Written by Jeremy Skinner (http://www.jeremyskinner.co.uk) and licensed under Apache 2.
- [.NET: Html Agility Pack](https://htmlagilitypack.codeplex.com/): This is an agile HTML parser that builds a read/write DOM and supports plain XPATH or XSLT (you actually don't HAVE to understand XPATH nor XSLT to use it, don't worry...). It is a .NET code library that allows you to parse "out of the web" HTML files. The parser is very tolerant with "real world" malformed HTML. The object model is very similar to what proposes System.Xml, but for HTML documents (or streams).
- [.NET: Base Class Libraries](https://bcl.codeplex.com/): The Base Class Libraries site hosts samples, previews, and prototypes from the BCL team.
This is a site for the BCL Team to get features to customers to try out without requiring a Beta or CTP of the .NET Framework. Our goal is to put generally useful functionality here, and to get feedback on it and have the chance to iterate on the design.
- [.NET: CommonLibrary.NET](https://commonlibrarynet.codeplex.com/): A collection of very reusable code and components in C# 4.0 ranging from ActiveRecord, Csv, Command Line Parsing, Configuration, Validation, Logging, Collections, Authentication, and much more. This is ideal for C# developer looking for a Utility library, Java developers looking for a C# version of Java Commons.
- [.NET: Craig-s-Utility-Library](http://jacraig.github.io/Craig-s-Utility-Library/): With .Net we have a number of built in classes and functions to help make a programmer's life easier, but let's face facts, they didn't think of everything. Craig's Utility Library tries to fill in some of those gaps (or at least the ones that I've run into). It comes with a couple hundred extension methods, built in data types such as a BTree, priority queue, ring buffer, etc. And that's just the DataTypes namespace. When you add it all up, Craig's Utility Library is one of the largest set of utilities for .Net out there.
- [.NET: Wintellect's Power Collections for .NET](http://powercollections.codeplex.com/): Power Collections makes heavy use of .NET Generics. The goal of the project is to provide generic collection classes that are not available in the .NET framework. Some of the collections included are the Deque, MultiDictionary, Bag, OrderedBag, OrderedDictionary, Set, OrderedSet, and OrderedMultiDictionary.
- [.NET: Humanizer](https://github.com/MehdiK/Humanizer): Humanizer meets all your .NET needs for manipulating and displaying strings, enums, dates, times, timespans, numbers and quantities
- [.NET: Wintellect PowerThreading](https://github.com/Wintellect/PowerThreading): Jeffrey Richter's Power Threading Library
- [.NET: Sigil](https://github.com/kevin-montrose/Sigil): A fail-fast validating helper for .NET CIL generation
- [.NET: Shielded](https://github.com/jbakic/Shielded): A strict and mostly lock-free Software Transactional Memory (STM) for .NET
- [.NET: NodaTime](https://github.com/nodatime/nodatime): A better date and time API for .NET
