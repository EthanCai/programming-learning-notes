# Books

参考：[Gobooks](https://github.com/dariubs/GoBooks)

- [An Introduction to Programming in Go](http://www.golang-book.com/): 一本介绍Go语言的书籍，内容非常简洁，便于快速掌握Go语法。
- [The Way to Go](http://book.douban.com/subject/10558892/):  a Thorough Introduction to the Go Programming Language 2012.3.8
- [Go语言编程](http://book.douban.com/subject/11577300/): 对个Go语言几个主要的主题进行了介绍，但内容不系统，不适合作为入门读物。更多见[豆瓣点评](http://book.douban.com/subject/11577300/reviews)
- [Go Programming Blueprints](http://book.douban.com/subject/26331858/): [亚马逊产品页面](http://www.amazon.com/Go-Programming-Blueprints-Development-Challenges/dp/1783988029/ref=sr_1_1)，Amazon评价很高，这本书介绍了很多高级主题
- [Network programming with Go](https://jan.newmarch.name/golang/)
- [Programming in Go](http://book.douban.com/subject/7070565/): [亚马逊产品页面](http://www.amazon.com/Programming-Go-Creating-Applications-Developers/dp/0321774639/ref=sr_1_4)，这本书的三个优点：High quality code samples；Idiomatic Go code；Details that aren't in the docs
- [The Go Programming Language Phrasebook](http://book.douban.com/subject/7952516/)
- [build-web-application-with-golang](https://github.com/astaxie/build-web-application-with-golang)

# Resources

官方网站：

- [Golang](http://golang.org/)
- [Golang国内镜像](http://docscn.studygolang.com/)
- [Go语言源代码](https://go.googlesource.com/go/)：在线查看Go语言源代码访问[这里](http://golang.org/src/)

语法：

- [A Tour of Go](https://tour.golang.org): The tour covers the most important features of the language
- [Go语言示例](https://gobyexample.com/): Go by Example is a hands-on introduction to Go using annotated example programs
- [The Go Programming Language Specification](https://golang.org/ref/spec)

Go Patterns:

- [Go Design Patterns](https://github.com/monochromegane/go_design_pattern)
- [go-resiliency](https://github.com/eapache/go-resiliency)
- [Go Examples of Common Patterns](https://github.com/jbuberel/go-patterns)
- [Go Patterns](https://github.com/tmrts/go-patterns): A curated collection of idiomatic design & application patterns for Go language.

Go Package：

- [GoDoc](https://godoc.org/): GoDoc hosts documentation for Go packages on Bitbucket, GitHub, Google Project Hosting and Launchpad.
    - [Go Walker](https://gowalker.org/): Go Walker 是一个可以在线生成并浏览 Go 项目 API 文档的 Web 服务器，目前已支持包括 GitHub 等代码托管平台
    - [Go Search](http://go-search.org/): 查找Go packages
- [Go Report Card](https://goreportcard.com): Report for golang package with `go vet`, `gocyclo`, `gofmt`, `golint`, `ineffassign`, `license`, `misspell`.
- [GoCover.io](https://gocover.io/): See code coverage of any Go package.

工具：

- [JSON to Go](https://mholt.github.io/json-to-go/): Convert JSON to Go struct

社区：

- [Golang社区](http://studygolang.com/)
- [Go邮件组](http://groups.google.com/group/golang-nuts)
- [Go的中文邮件组](http://groups.google.com/group/golang-china)

资料收集：

- [Golang资料集](https://github.com/ty4z2008/Qix/blob/master/golang.md)
- [Golang资料收集](https://github.com/wonderfo/wonderfogo/wiki)

# 文章、演示文档、视频、示例

- [Go Concurrency Patterns - Rob Pike](https://talks.golang.org/2012/concurrency.slide)
    - [Google I/O 2012 - Go Concurrency Patterns - Rob Pike](https://www.youtube.com/watch?v=f6kdp27TYZs)
- [OOPs in Go by William Kennedy](https://www.youtube.com/watch?v=gRpUfjTwSOo)
- [Golang Memory Module](http://golang.org/ref/mem)

# 学习路径

1. 安装Go
    - 参考[Get Started](http://golang.org/doc/install)安装Golang runtime，如果OS X通过Homebrew安装
    - IDE
        - 使用Atom，需要安装[Go-Plus Package](https://atom.io/packages/go-plus)
        - 使用IDEA Community，需要安装[go-lang-idea-plugin](https://github.com/go-lang-plugin-org/go-lang-idea-plugin/wiki/Documentation), 文档见[这里](https://github.com/go-lang-plugin-org/go-lang-idea-plugin/wiki/Documentation)
1. 练习搭建基本的Workspace，并熟悉Workspace的结构、Go代码结构、编写基本的单元测试、`Go fmt/build/install/run/test`等命名的使用
    - [How to Write Go Code](http://golang.org/doc/code.html)
    - [Go命令文档](http://golang.org/doc/cmd)
1. 编写Golang程序
    - 熟悉Golang的编码规范，[Effective Go - Go语言编码规范](http://golang.org/doc/effective_go.html)
    - 熟悉Golang标准库，[Go语言Package文档](http://golang.org/pkg/)
1. 工程管理
    - 不建议创建多个Workspace，管理起来增加不必要的麻烦
        - 如果想配置多个Workspace，按照如下方法配置：
            - 主要配置方法参考[Go environment setup](http://blog.tideland.biz/2013-07-09-go-environment-setup)
            - `GoPath`支持设置多个目录；如果`GoPath`设置了多个路径，执行`go get`命令，会默认下载到`GoPath`中第一个路径中
    - 代码检查
        - [Go metal linter](https://github.com/alecthomas/gometalinter): Concurrently run Go lint tools and normalise their output
    - 编译
        - [Package Management Tools - Golang Wiki](https://github.com/golang/go/wiki/PackageManagementTools)
        - Godep和GoPM的区别：
            - 使用GoPM方式管理引用的第三方package，引用第三方package的列表保存在`/.gopmfile`文件中，如[这里](https://github.com/gogits/gogs/blob/master/.gopmfile)
            - 使用Godep方式管理引用的第三方package，引用的第三方package的列表保存在`/Godeps/Godeps.json`文件中，第三方package源代码也需要包含在项目代码中，保存在`/Godeps/_workspace/src`目录下，参考[etcd项目结构](https://github.com/coreos/etcd)
            - GoPM管理方式更优雅；GoPM的管理命令也比Godep更易用；由于GoPM服务架设在中国，所以在国内使用GoPM访问也更快；但是GoPM管理方式存在安全问题，如果GoPM服务挂掉或者第三方package代码库变更，那么也就无法下载引用的第三方package，从安全角度对于企业是不可接受的
            - Godeps管理方式虽然不存在安全问题，但是如果第三方package有更新，那么更新`/Godeps`目录下的第三方package代码也不方便
        - 工具
            - 标准`go get`
            - [Godep](https://github.com/tools/godep): dependency tool for go
            - [Glide](https://glide.sh/): Vendor Package Management for Golang
            - [Go vendor](https://github.com/kardianos/govendor): Go vendor tool that works with the standard vendor file.
    - 打包
        - [gb](https://github.com/constabulary/gb): the project based build tool for Go



## Go语言标准库

Go标准库可以大致按其中库的功能进行以下分类,这个分类比较简单,不求准确,但求能 够帮助开发者根据自己模糊的需求更快找到自己需要的包。

- 输入输出。这个分类包括二进制以及文本格式在屏幕、键盘、文件以及其他设备上的输入输出等,比如二进制文件的读写。对应于此分类的包有bufio、fmt、io、io/ioutil、log、log/syslog、flag等,其中flag用于处理命令行参数。
- 文本处理。这个分类包括字符串和文本内容的处理,比如字符编码转换等。对应于此分类的包有encoding、bytes、strings、strconv、text、mime、unicode、regexp、index和path等。其中path用于处理路径字符串。
- 网络。这个分类包括开发网络程序所需要的包,比如Socket编程和网站开发等。对应于此分类的包有:net、http和expvar等。
- 系统。这个分类包含对系统功能的封装,比如对操作系统的交互以及原子性操作等。对应于此分类的包有os、syscall、sync、time和unsafe等。

更多的标准库说明参考[Go语言Package文档](http://golang.org/pkg/)


### 输入输出

- [fmt](https://golang.org/pkg/fmt/)
- [io](https://golang.org/pkg/io/)
- [io/ioutil](https://golang.org/pkg/io/ioutil/)
- [bufio](https://golang.org/pkg/bufio/)
- [log](https://golang.org/pkg/log/)
- [log/syslog](https://golang.org/pkg/log/syslog/)
- [flag](https://golang.org/pkg/flag/)

### 文本处理

- [encoding](https://golang.org/pkg/encoding/)
- [bytes](https://golang.org/pkg/bytes/)
- [strings](https://golang.org/pkg/strings/)
- [strconv](https://golang.org/pkg/strconv/)
- [text](https://golang.org/pkg/)
- [mime](https://golang.org/pkg/mime/)
- [regexp](https://golang.org/pkg/regexp/)
- [index](https://golang.org/pkg/index/)
- [path](https://golang.org/pkg/path/)

### 网络

- [net](https://golang.org/pkg/net/)
- [HTTP](https://golang.org/pkg/net/http/)
- [RPC](https://golang.org/pkg/net/rpc/)
- [expvar](https://golang.org/pkg/expvar/)

### 系统

- [os](https://golang.org/pkg/os/)
- [syscall](https://golang.org/pkg/syscall/)
- [sync](https://golang.org/pkg/sync/)
- [time](https://golang.org/pkg/time/)
- [unsafe](https://golang.org/pkg/unsafe/)

------------------------------

# 参考项目列表

- [Golang Projects - OSChina](http://www.oschina.net/project/lang/358/go)
- [Awesome Go](https://github.com/avelino/awesome-go)


# Basic Projects

## Project Dependency and Build

- [goviz](https://github.com/hirokidaichi/goviz): a visualization tool for golang project dependency

## Language

- [Delve](https://github.com/derekparker/delve/): Delve is a debugger for the Go programming language.
- [otto](https://github.com/robertkrimen/otto): A JavaScript interpreter in Go (golang)
- [gopherjs](https://github.com/gopherjs/gopherjs): A compiler from Go to JavaScript for running Go code in a browser

## Dev

- [gorc](https://github.com/stretchr/gorc): Recursive go testing, done better.
- [gvm](https://github.com/moovweb/gvm): Go Version Manager
- [Wide](https://github.com/b3log/wide): A Web-based IDE for Teams using Go programming language/Golang
- [http2curl](https://github.com/moul/http2curl):  Convert Golang's http.Request to CURL command line

## Test

- [Testify](https://github.com/stretchr/testify): A sacred extension to the standard go testing package
- [Go frisby](https://github.com/verdverm/frisby): API testing framework inspired by frisby-js
- [httpexpect](https://github.com/gavv/httpexpect): End-to-end HTTP and REST API testing for Go.

## Terminal

- [odin](https://github.com/jwaldrip/odin): A go-lang library to help build self documenting command line applications.
- [go-flags](https://github.com/jessevdk/go-flags): go command line option parser
- [kingpin](http://gopkg.in/alecthomas/kingpin.v2):

## Text Processing & Search

- [bleve](https://github.com/blevesearch/bleve): A modern text indexing library for go
- [Pholcus](https://github.com/henrylee2cn/pholcus): Pholcus（幽灵蛛）是一款纯Go语言编写的高并发、分布式、重量级爬虫软件，支持单机、服务端、客户端三种运行模式，拥有Web、GUI、命令行三种操作界面；规则简单灵活、批量任务并发、输出方式丰富（mysql/mongodb/csv/excel等）、有大量Demo共享；同时她还支持横纵向两种抓取模式，支持模拟登录和任务暂停、取消等一系列高级功能
- [sego](https://github.com/huichen/sego): Go中文分词
- [goquery](https://github.com/PuerkitoBio/goquery): goquery brings a syntax and a set of features similar to jQuery to the Go language. It is based on Go's net/html package and the CSS Selector library cascadia. Since the net/html parser returns nodes, and not a full-featured DOM tree, jQuery's stateful manipulation functions (like height(), css(), detach()) have been left off.

## Network

- [DNS library in Go](https://github.com/miekg/dns): DNS library in Go
- [GRPC](http://www.grpc.io/): A high performance, open source, general RPC framework that puts mobile and HTTP/2 first.
- [fasthttp](https://github.com/valyala/fasthttp): Fast HTTP package for Go. Tuned for high performance. Zero memory allocations in hot paths. Up to 10x faster than net/http.
- [link](https://github.com/funny/link): Go语言网络层脚手架
- [tus](http://www.oschina.net/p/tus): 一个开放的协议实现了客户端和服务器之间可恢复的文件上传协议

## JSON

- [go-simplejson](https://github.com/bitly/go-simplejson): a Go package to interact with arbitrary JSON
- [Jason](https://github.com/antonholmquist/jason): Easy-to-use JSON Library for Go
- [jsonpath](https://github.com/yalp/jsonpath): a (partial) implementation in Go based on [Stefan Goener JSON Path](http://goessner.net/articles/JsonPath/)
- [gojsonschema](https://github.com/xeipuuv/gojsonschema): An implementation of JSON Schema, based on IETF's draft v4 - Go language
- [gojsondiff](https://github.com/yudai/gojsondiff/): Go JSON Diff

## Data Access

- [gorm](https://github.com/jinzhu/gorm): The fantastic ORM library for Golang, aims to be developer friendly
- [xorm](https://github.com/go-xorm/xorm): Simple and Powerful ORM for Go, support mysql/sqlite3/postgres/mssql/oracle/tidb/ql
- [Go-MySQL-Driver](https://github.com/go-sql-driver/mysql): Go-MySQL-Driver is a lightweight and fast MySQL-Driver for Go's (golang) database/sql package

## Monitor & Alert

- [bosun](https://github.com/bosun-monitor/bosun): Time Series Alerting Framework

## Log

- [logrus](https://github.com/Sirupsen/logrus): Structured, pluggable logging for Go.
- [Apex/log](https://github.com/apex/log): Structured logging package for Go.

## Message Queue

- [NSQ](http://nsq.io/): A realtime distributed messaging platform

## Web Framework

![](https://raw.githubusercontent.com/iris-contrib/website/cf71811e6acb2f9bf1e715e25660392bf090b923/assets/benchmark_horizontal_transparent.png)

**Web Frameworks in the chart:**

- [Beego](http://beego.me/): 一个使用 Go 的思维来帮助您构建并开发 Go 应用程序的开源框架
- [Gin Web Framework](https://github.com/gin-gonic/gin): Gin is a web framework written in Golang. It features a martini-like API with much better performance, up to 40 times faster thanks to httprouter. If you need performance and good productivity, you will love Gin.
- [Iris](https://github.com/kataras/iris): The fastest web framework for Go in (THIS) earth
- [martini](https://github.com/go-martini/martini): Martini is a powerful package for quickly writing modular web applications/services in Golang.
- [revel](http://revel.github.io/): A high-productivity web framework for the Go language.

**Other Web Frameworks:**

- [tango](https://github.com/lunny/tango): Micro & pluggable web framework for Go
- [webgo](https://github.com/hoisie/web): web.go is the simplest way to write web applications in the Go programming language. It's ideal for writing simple, performant backend web services.

## Micro Services

- [gokit](https://github.com/go-kit/kit): Go kit is a distributed programming toolkit for building microservices in large organizations. We solve common problems in distributed systems, so you can focus on your business logic.
- [goa](http://goa.design/): goa is a Go framework for developing RESTful microservices.
- [micro](https://github.com/micro/micro): A microservice toolkit
- [Gizmo Microservice Toolkit](https://github.com/NYTimes/gizmo): This toolkit provides packages to put together server and pubsub daemons

## Other Web Related Projects

- [restful](https://github.com/devcamcar/restful): Restful HTTP Client package in golang
- [Gorilla web toolkit](http://www.gorillatoolkit.org/): Gorilla is a web toolkit for the Go programming language.
- [GoRazor](https://github.com/sipin/gorazor): Razor view engine for Golang
- [Webhook](https://github.com/adnanh/webhook): webhook is a lightweight configurable tool written in Go, that allows you to easily create HTTP endpoints (hooks) on your server, which you can use to execute configured commands.

## Cache

- [Groupcahe](https://github.com/golang/groupcache): groupcache is a caching and cache-filling library, intended as a replacement for memcached in many cases.

## Server-side Push Service for Mobile App

- [uniqush-push](https://github.com/uniqush/uniqush-push): Uniqush is a free and open source software which provides a unified push service for server-side notification to apps on mobile devices.

## AWS

- [apex](https://github.com/apex/apex): Minimal AWS Lambda function manager with Go support.

## IoT

- [Gobot](http://gobot.io/): Gobot is a framework for robotics, physical computing, and the Internet of Things, written in the Go programming language.

## Data Structure

- [queue](https://github.com/eapache/queue):  not thread-safe queue
- [safemap](https://github.com/pcrawfor/safemap): A golang channel based access object for shared use of a map of arbitrary objects

## Misc

- [robpike.io/filter](https://godoc.org/robpike.io/filter): Package filter contains utility functions for filtering slices through the distributed application of a filter function.
- [Parallel](https://github.com/wangkuiyi/parallel): Some OpenMP like syntax for Go
- [goerlang/node](https://github.com/goerlang/node): Implementation of Erlang node
- [topicai/candy](https://github.com/topicai/candy): candy includes a set of easy-to-use Go facilities.


# System Administration

## Service Orchestration and Management

- [serf](https://github.com/hashicorp/serf): Service orchestration and management tool

## Monitor

- [Open-Falcon企业级监控系统解决方案](http://open-falcon.com/): Open-Falcon 是小米运维部开源的一款互联网企业级监控系统解决方案.
- [Prometheus](https://github.com/prometheus/prometheus): Prometheus is a systems and service monitoring system. It collects metrics from configured targets at given intervals, evaluates rule expressions, displays the results, and can trigger alerts if some condition is observed to be true.

## Network

- [toxy](https://github.com/h2non/toxy): Hackable HTTP proxy to simulate server failure scenarios and unexpected network conditions
- [Tyk API Gateway](https://github.com/lonelycode/tyk): Tyk is a lightweight, open source API Gateway and enables you to control who accesses your API, when they access it and how they access it. Tyk will also record detailed analytics on how your users are interacting with your API and when things go wrong.
- [Gor](https://github.com/buger/gor): Gor is an open-source tool for capturing and replaying live HTTP traffic into a test environment in order to continuously test your system with real data. It can be used to increase confidence in code deployments, configuration changes and infrastructure changes.
- [Seesaw](https://github.com/google/seesaw): Seesaw v2 is a Linux Virtual Server (LVS) based load balancing platform.

## Job Schedule

- [dkron](https://github.com/victorcoder/dkron): Distributed, fault tolerant job scheduling system
- [webcron](https://github.com/codeskyblue/webcron): A new crontab that have a web page in order to replace the original crontab. Now it can try on test.
- [kingtask](https://github.com/kingsoft-wps/kingtask): A lightweight asynchronous timing task system powered by Go
- [cron](https://github.com/robfig/cron): a cron library for go

## Code Repository

- [Gogs](http://gogs.io/): 极易搭建的自助 Git 服务
- [Gitea - a self-hosted Git service](https://github.com/go-gitea/gitea)
- [git - appraise](https://github.com/google/git-appraise): Distributed Code Review For Git

## Distributed ID Generator

- [sonyflake](https://github.com/sony/sonyflake): A distributed unique ID generator inspired by Twitter's Snowflake

## Database

- [tidb](https://github.com/pingcap/tidb): TiDB is a distributed NewSQL database compatible with MySQL protocol

## Backup

- [restic](https://github.com/restic/restic): restic backup program
- [syncthing](https://github.com/syncthing/syncthing): Open Source Continuous File Synchronization

## Terminal Enhancement

- [termui- Golang terminal dashboard](https://github.com/gizak/termui)
- [GoTTY](https://github.com/yudai/gotty): Share your terminal as a web application

## Work Efficiency

- [s](https://github.com/zquestz/s): Open a web search in your terminal.


# Business Applications

## API & SDK

- [weixinmp](https://github.com/sidbusy/weixinmp): 微信公众平台SDK for Go

## 3D

- [ln](https://github.com/fogleman/ln): ln is a vector-based 3D renderer written in Go. It is used to produce 2D vector graphics (think SVGs) depicting 3D scenes. The output of an OpenGL pipeline is a rastered image. The output of ln is a set of 2D vector paths.

## Authentication

- [captcha](https://github.com/jianxinio/captcha): Golang实现的验证码服务
- [Go OTP](https://github.com/hgfischer/go-otp): Package go-otp implements one-time-password generators used in 2-factor authentication systems like RSA-tokens. Currently this supports both HOTP (RFC-4226), TOTP (RFC-6238) and Base32 encoding (RFC-3548) for Google Authenticator compatibility
    - [Go-otpserver](https://github.com/skyjia/go-otpserver): A golang version OTP server.

## Misc

- [Gor](https://github.com/wendal/gor): Golang编写的静态博客引擎
- [heim](https://github.com/euphoria-io/heim): A real-time community platform
- [Mattermost](https://github.com/mattermost/platform): Mattermost is an open-source team communication service. It brings team messaging and file sharing into one place, accessible across PCs and phones, with archiving and search.
- [ohlala](https://github.com/QLeelulu/ohlala): 觅链，一个具有社会化媒体属性的链接分享与评论平台。类似Reddit
- [Pachyderm](https://github.com/pachyderm/pachyderm): Containerized Data Analytics


--------------------------------

# FAQ

## What is difference between Goroutines vs OS threads?

参考：

- [What-is-difference-between-Goroutines-vs-OS-threads](http://www.quora.com/What-is-difference-between-Goroutines-vs-OS-threads)
- [goroutine背后的系统知识](http://www.infoq.com/cn/articles/knowledge-behind-goroutine)
- [golang的goroutine是如何实现的?](http://www.zhihu.com/question/20862617)
- [Concurrency, Goroutines and GOMAXPROCS](http://www.goinggo.net/2014/01/concurrency-goroutines-and-gomaxprocs.html)
- [Green threads](http://www.wikiwand.com/en/Green_threads)

The Go runtime multiplexes a potentially large number of goroutines onto a smaller number of OS threads, and goroutines blocked on I/O are handled efficiently using epoll or similar facilities.  Goroutines have tiny stacks that grow as needed, so it is practical to have hundreds of thousands of goroutines in your program. This allows the programmer to use concurrency to structure their program without being overly concerned with thread overhead.

## Go语言和其它语言的比较

参考：

- [我为什么从python转向go](http://www.jianshu.com/p/afa14e631930)
- [Node.js vs Golang: Battle of the Next-Gen Languages](http://www.hostingadvice.com/blog/nodejs-vs-golang/)

## Go语言主要版本和版本变更内容是哪些？

参考：

- [Release History](http://golang.org/doc/devel/release.html)
