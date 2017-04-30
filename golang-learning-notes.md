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
