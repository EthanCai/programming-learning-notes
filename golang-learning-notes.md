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
            - [Glide](https://glide.sh/): Vendor Package Management for Golang
            - [gb](https://getgb.io/): A project based build tool for the Go programming language.
            - [Godep](https://github.com/tools/godep): dependency tool for go
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

------------------------------

# 参考项目列表

- [Golang Projects - OSChina](http://www.oschina.net/project/lang/358/go)
- [Awesome Go](https://github.com/avelino/awesome-go)
- [Golang libs](https://golanglibs.com/o)
- [Go语言(golang)开源项目大全](http://www.open-open.com/lib/view/open1396063913278.html)


# Basic Projects

## Libs Improve Development Efficiency

- [pointer](https://github.com/AlekSi/pointer): Go package pointer provides helpers to get pointers to values of build-in types.
- [robpike.io/filter](https://godoc.org/robpike.io/filter): Package filter contains utility functions for filtering slices through the distributed application of a filter function.
- [topicai/candy](https://github.com/topicai/candy): candy includes a set of easy-to-use Go facilities.
- [facebook inject](https://godoc.org/github.com/facebookgo/inject): Package inject provides a reflect based injector. A large application built with dependency injection in mind will typically involve the boring work of setting up the object graph. This library attempts to take care of this boring work by creating and connecting the various objects.

## Data Structure

- [queue](https://github.com/eapache/queue):  not thread-safe queue
- [safemap](https://github.com/pcrawfor/safemap): A golang channel based access object for shared use of a map of arbitrary objects

## Terminal

- [odin](https://github.com/jwaldrip/odin): A go-lang library to help build self documenting command line applications.
- [go-flags](https://github.com/jessevdk/go-flags): go command line option parser
- [kingpin](http://gopkg.in/alecthomas/kingpin.v2):

## Network

- [DNS library in Go](https://github.com/miekg/dns): DNS library in Go
- [fasthttp](https://github.com/valyala/fasthttp): Fast HTTP package for Go. Tuned for high performance. Zero memory allocations in hot paths. Up to 10x faster than net/http.
- [link](https://github.com/funny/link): Go语言网络层脚手架
- [tus](http://www.oschina.net/p/tus): 一个开放的协议实现了客户端和服务器之间可恢复的文件上传协议
- [sleuth](https://github.com/ursiform/sleuth): sleuth is a Go library that provides master-less peer-to-peer autodiscovery and RPC between HTTP services that reside on the same network. It works with minimal configuration and provides a mechanism to join a local network both as a client that offers no services and as any service that speaks HTTP. Its primary use case is for microservices on the same network that make calls to one another.
- [kcp-go](https://github.com/xtaci/kcp-go): A full-featured reliable UDP communication library
    - [kcptun](https://github.com/xtaci/kcptun): an extremely simple & fast udp tunnel based on kcp protocol
- [centrifugo](https://github.com/centrifugal/centrifugo): Real-time messaging (Websockets or SockJS) server in Go
- [http2curl](https://github.com/moul/http2curl):  Convert Golang's http.Request to CURL command line

## JSON

- [go-simplejson](https://github.com/bitly/go-simplejson): a Go package to interact with arbitrary JSON
- [Jason](https://github.com/antonholmquist/jason): Easy-to-use JSON Library for Go
- [jsonpath](https://github.com/yalp/jsonpath): a (partial) implementation in Go based on [Stefan Goener JSON Path](http://goessner.net/articles/JsonPath/)
- [gojsonschema](https://github.com/xeipuuv/gojsonschema): An implementation of JSON Schema, based on IETF's draft v4 - Go language
- [gojsondiff](https://github.com/yudai/gojsondiff/): Go JSON Diff

## Log

- [zap](https://github.com/uber-go/zap): Fast, structured, leveled logging in Go
- [logrus](https://github.com/Sirupsen/logrus): Structured, pluggable logging for Go.
- [Apex/log](https://github.com/apex/log): Structured logging package for Go.
- [stack](https://github.com/facebookgo/stack): provides utilities to capture and pass around stack traces.

## Web Related Projects

### Web Framework

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

### Micro Services

- [gokit](https://github.com/go-kit/kit): Go kit is a distributed programming toolkit for building microservices in large organizations. We solve common problems in distributed systems, so you can focus on your business logic.
- [goa](http://goa.design/): goa is a Go framework for developing RESTful microservices.
- [micro](https://github.com/micro/micro): A microservice toolkit
- [Gizmo Microservice Toolkit](https://github.com/NYTimes/gizmo): This toolkit provides packages to put together server and pubsub daemons

### Other

- [restful](https://github.com/devcamcar/restful): Restful HTTP Client package in golang
- [Gorilla web toolkit](http://www.gorillatoolkit.org/): Gorilla is a web toolkit for the Go programming language.
- [GoRazor](https://github.com/sipin/gorazor): Razor view engine for Golang
- [Webhook](https://github.com/adnanh/webhook): webhook is a lightweight configurable tool written in Go, that allows you to easily create HTTP endpoints (hooks) on your server, which you can use to execute configured commands.
- [form](https://github.com/go-playground/form): Decodes url.Values into struct values and Encodes struct values into url.Values. Dual Array and Full map support.

## Scheduler

- [cron](https://github.com/robfig/cron): a cron library for go
- [gocron](https://github.com/jasonlvhit/gocron): A Golang Job Scheduling Package.
- [jobber](https://github.com/dshearer/jobber): A replacement for cron, with sophisticated status-reporting and error-handling.
- [hashicorp/Nomad](https://github.com/hashicorp/nomad): Nomad is a cluster manager, designed for both long lived services and short lived batch processing workloads. Developers use a declarative job specification to submit work, and Nomad ensures constraints are satisfied and resource utilization is optimized by efficient task packing
- [scheduler](https://github.com/carlescere/scheduler): Job scheduling made easy.
- [workq](https://github.com/iamduo/workq): Workq is a job scheduling server strictly focused on simplifying job processing and streamlining coordination. It can run jobs in blocking foreground or non-blocking background mode.

## Authentication

- [captcha](https://github.com/jianxinio/captcha): Golang实现的验证码服务
- [Go OTP](https://github.com/hgfischer/go-otp): Package go-otp implements one-time-password generators used in 2-factor authentication systems like RSA-tokens. Currently this supports both HOTP (RFC-4226), TOTP (RFC-6238) and Base32 encoding (RFC-3548) for Google Authenticator compatibility
    - [Go-otpserver](https://github.com/skyjia/go-otpserver): A golang version OTP server.

## Communication

- [heim](https://github.com/euphoria-io/heim): A real-time community platform
- [Mattermost](https://github.com/mattermost/platform): Mattermost is an open-source team communication service. It brings team messaging and file sharing into one place, accessible across PCs and phones, with archiving and search.

## Utilities

- [apex](https://github.com/apex/apex): Minimal AWS Lambda function manager with Go support.
- [clipboard](https://github.com/atotto/clipboard): Provide copying and pasting to the Clipboard for Go.
- [fsnotify](https://github.com/fsnotify/fsnotify): File system notifications for Go.
- [i18n4go](https://github.com/maximilien/i18n4go): This is a general purpose internationalization (i18n) tooling for Go language (Golang) programs. It allows you to prepare Go language code for internationalization and localization (l10n).
- [uniqush-push](https://github.com/uniqush/uniqush-push): Uniqush is a free and open source software which provides a unified push service for server-side notification to apps on mobile devices.
- [goerlang/node](https://github.com/goerlang/node): Implementation of Erlang node
- [Parallel](https://github.com/wangkuiyi/parallel): Some OpenMP like syntax for Go
- [serf](https://github.com/hashicorp/serf): Service orchestration and management tool
- [ln](https://github.com/fogleman/ln): ln is a vector-based 3D renderer written in Go. It is used to produce 2D vector graphics (think SVGs) depicting 3D scenes. The output of an OpenGL pipeline is a rastered image. The output of ln is a set of 2D vector paths.
- [restic](https://github.com/restic/restic): restic backup program
- [syncthing](https://github.com/syncthing/syncthing): Open Source Continuous File Synchronization
- [weixinmp](https://github.com/sidbusy/weixinmp): 微信公众平台SDK for Go
