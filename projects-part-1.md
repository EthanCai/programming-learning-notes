<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Projects about Application Software Development](#projects-about-application-software-development)
	- [Compiler](#compiler)
	- [REPL](#repl)
	- [Language Converter](#language-converter)
	- [Interpreter](#interpreter)
	- [Debugger](#debugger)
	- [Analyzer](#analyzer)
	- [Profiling](#profiling)
	- [Web Servers & Application Servers](#web-servers-application-servers)
	- [Application Frameworks](#application-frameworks)
	- [Template Engine](#template-engine)
	- [GUI Framework](#gui-framework)
	- [Asynchronous Programming Framework](#asynchronous-programming-framework)
	- [Web Socket](#web-socket)
	- [Network](#network)
	- [Thread & Coroutine](#thread-coroutine)
	- [Reflect & IoC](#reflect-ioc)
	- [Logging](#logging)
	- [Data Access](#data-access)
	- [Serialization & Deserialization](#serialization-deserialization)
	- [Command Line](#command-line)
	- [File](#file)
	- [Image Processing](#image-processing)
	- [Audio & Video](#audio-video)
	- [Computer Vision](#computer-vision)
	- [Authentication & Authorization](#authentication-authorization)
	- [Office Documents](#office-documents)
	- [Misc Libraries](#misc-libraries)

<!-- /TOC -->

# Projects about Application Software Development

## Compiler

- [LLVM](http://www.llvm.org/): The LLVM Project is a collection of modular and reusable compiler and toolchain technologies. Despite its name, LLVM has little to do with traditional virtual machines. The name "LLVM" itself is not an acronym; it is the full name of the project.
- [Java: OpenJDK](http://openjdk.java.net/): open-source implementation of the Java Platform, Standard Edition
- [Java: Oracle JDK](http://www.oracle.com/technetwork/java/javase/overview/index.html): N/A
- [Java: Eclipse OpenJ9](http://www.eclipse.org/openj9/): IBM已经开源自己的JDK作为Eclipse OpenJ9

## REPL

- Online REPL
  - [repl.it](https://repl.it/): Multiple languages repl
  - [Go Playground](https://play.golang.org/)
  - [JS Fiddle](https://jsfiddle.net/)
- Go
  - [gore](https://github.com/motemen/gore)
  - [gosh](https://github.com/mkouhei/gosh)
  - [igo](https://github.com/sbinet/igo)

## Language Converter

- [gopherjs](https://github.com/gopherjs/gopherjs): A compiler from Go to JavaScript for running Go code in a browser
- [Grumpy](https://github.com/google/grumpy): Grumpy is a Python to Go source code transcompiler and runtime.

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

## Web Servers & Application Servers

- [Nginx](http://wiki.nginx.org/Main): a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
    - [OpenResty](http://openresty.org/): OpenResty (aka. ngx_openresty) is a full-fledged web application server by bundling the standard Nginx core, lots of 3rd-party Nginx modules, as well as most of their external dependencies.
    - [Tengine](http://tengine.taobao.org/): Tengine是由淘宝网发起的Web服务器项目。它在Nginx的基础上，针对大访问量网站的需求，添加了很多高级功能和特性。Tengine的性能和稳定性已经在大型的网站如淘宝网，天猫商城等得到了很好的检验。它的最终目标是打造一个高效、稳定、安全、易用的Web平台。
    - [VeryNginx](https://github.com/alexazhou/VeryNginx): 功能强大并且拥有对人类友好界面的Nginx, 提供防火墙，自定义行为和统计功能
- [lightttpd](http://www.lighttpd.net/): Security, speed, compliance, and flexibility -- all of these describe lighttpd (pron. lighty) which is rapidly redefining efficiency of a webserver; as it is designed and optimized for high performance environments. With a small memory footprint compared to other web-servers, effective management of the cpu-load, and advanced feature set (FastCGI, SCGI, Auth, Output-Compression, URL-Rewriting and many more) lighttpd is the perfect solution for every server that is suffering load problems. And best of all it's Open Source licensed under the revised BSD license.
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

## Template Engine

- Go
  - full featured template engines
    * [Ace](https://github.com/yosssi/ace)
    * [Amber](https://github.com/eknkc/amber)
    * [Go](https://golang.org/pkg/html/template)
    * [Handlebars](https://github.com/aymerick/raymond)
    * [Kasia](https://github.com/ziutek/kasia.go)
    * [Mustache](https://github.com/hoisie/mustache)
    * [Pongo2](https://github.com/flosch/pongo2)
    * [Soy](https://github.com/robfig/soy)
    * [Jet](https://github.com/CloudyKit/jet)
  - precompilation to Go code
    * [ego](https://github.com/benbjohnson/ego)
    * [egon](https://github.com/commondream/egon)
    * [egonslinso](https://github.com/SlinSo/egon)
    * [ftmpl](https://github.com/tkrajina/ftmpl)
    * [Gorazor](https://github.com/sipin/gorazor)
    * [Quicktemplate](https://github.com/valyala/quicktemplate)
    * [Hero](https://github.com/shiyanhui/hero)

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
  - [Python: RxPY](https://github.com/ReactiveX/RxPY)
  - [C#: Rx.NET](https://github.com/Reactive-Extensions/Rx.NET)
  - C#(Unity): UniRx
  - Scala: RxScala
  - Clojure: RxClojure
  - C++: RxCpp
  - Lua: RxLua
  - Ruby: Rx.rb
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

## Reflect & IoC

- [Go: facebookgo/inject](https://github.com/facebookgo/inject): Package inject provides a reflect based injector.
- [Go: reflections](https://github.com/oleiade/reflections): Golang high level abstractions over reflect library
- [Go: mapstructure](https://github.com/mitchellh/mapstructure): Go library for decoding generic map values into native Go structures.
- [Go: copystructure](https://github.com/mitchellh/copystructure): Go (golang) library for deep copying values in Go.
- [Go: reflectwalk](https://github.com/mitchellh/reflectwalk): reflectwalk is a Go library for "walking" complex structures, similar to walking a filesystem.
- [Go: robpike.io/filter](https://godoc.org/robpike.io/filter): Package filter contains utility functions for filtering slices through the distributed application of a filter function.

## Logging

- [Go: zap](https://github.com/uber-go/zap): Fast, structured, leveled logging in Go
- [Go: logrus](https://github.com/Sirupsen/logrus): Structured, pluggable logging for Go.
- [Go: Apex/log](https://github.com/apex/log): Structured logging package for Go.
- [Go: stack](https://github.com/facebookgo/stack): provides utilities to capture and pass around stack traces.

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

## Serialization & Deserialization

- [Go: go-simplejson](https://github.com/bitly/go-simplejson): a Go package to interact with arbitrary JSON
- [Go: Jason](https://github.com/antonholmquist/jason): Easy-to-use JSON Library for Go
- [Go: jsonpath](https://github.com/yalp/jsonpath): a (partial) implementation in Go based on [Stefan Goener JSON Path](http://goessner.net/articles/JsonPath/)
- [Go: gojsonschema](https://github.com/xeipuuv/gojsonschema): An implementation of JSON Schema, based on IETF's draft v4 - Go language
- [Go: gojsondiff](https://github.com/yudai/gojsondiff/): Go JSON Diff
- [Java: fastjson](https://github.com/alibaba/fastjson): A fast JSON parser/generator for Java

## Command Line

- [Go: viper](https://github.com/spf13/viper): Go configuration with fangs
- [Go: go-flags](https://github.com/jessevdk/go-flags): go command line option parser
- [Go: kingpin](https://github.com/alecthomas/kingpin): A Go (golang) command line and flag parser

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

## Authentication & Authorization

- [Go: captcha](https://github.com/jianxinio/captcha): Golang实现的验证码服务
- [Go: Go OTP](https://github.com/hgfischer/go-otp): Package go-otp implements one-time-password generators used in 2-factor authentication systems like RSA-tokens. Currently this supports both HOTP (RFC-4226), TOTP (RFC-6238) and Base32 encoding (RFC-3548) for Google Authenticator compatibility
    - [Go-otpserver](https://github.com/skyjia/go-otpserver): A golang version OTP server.

## Office Documents

- [Go: excelize](https://github.com/360EntSecGroup-Skylar/excelize): Golang library for reading and writing Microsoft Excel™ (XLSX) files.
- [Go: xlsx](https://github.com/tealeg/xlsx): Google Go (golang) library for reading and writing XLSX files.
- [Go: gooxml](https://github.com/baliance/gooxml): Pure go library for creating Office Open/OOXML/ECMA-376 documents (.docx, .xlsx, .pptx) 

## Misc Libraries

- [C++: Boost](http://www.boost.org/)
- [C++: Abseil](https://abseil.io/)
- [Go: null](https://github.com/guregu/null): reasonable handling of nullable values
- [Go: pointer](https://github.com/AlekSi/pointer): Go package pointer provides helpers to get pointers to values of build-in types.
- [Go: queue](https://github.com/eapache/queue):  not thread-safe queue
- [Go: safemap](https://github.com/pcrawfor/safemap): A golang channel based access object for shared use of a map of arbitrary objects
- [Go: i18n4go](https://github.com/maximilien/i18n4go): This is a general purpose internationalization (i18n) tooling for Go language (Golang) programs. It allows you to prepare Go language code for internationalization and localization (l10n).
