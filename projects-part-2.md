<!-- MDTOC maxdepth:6 firsth1:1 numbering:0 flatten:0 bullets:1 updateOnSave:1 -->

- [Projects about Distributed Architecture](#projects-about-distributed-architecture)
   - [Open Platform](#open-platform)
   - [Distributed Application Framework](#distributed-application-framework)
   - [Data Exchange Format](#data-exchange-format)
   - [RPC](#rpc)
   - [Service Bus](#service-bus)
   - [Messsage Queue](#messsage-queue)
   - [Job Schedule](#job-schedule)
   - [Load Balance](#load-balance)
   - [API Gateway](#api-gateway)
   - [API Proxy](#api-proxy)
   - [Reverse Proxy](#reverse-proxy)
   - [Distributed File System](#distributed-file-system)
   - [Configuration Management](#configuration-management)
   - [Service Discovery, Name Service](#service-discovery-name-service)
   - [DNS Server](#dns-server)
   - [Circuit Breaker](#circuit-breaker)
   - [Distributed Tracing](#distributed-tracing)
   - [Other](#other)

<!-- /MDTOC -->

# Projects about Distributed Architecture

## Open Platform

- [Istio](https://istio.io/): An open platform to connect, manage, and secure microservices

## Distributed Application Framework

- [Go: go-kit](https://github.com/go-kit): A standard library for microservices.
- [Go: micro](https://github.com/micro): A microservice toolkit for distributed systems development
- [Go: go-chassis](https://github.com/ServiceComb): Go-Chassis is a Software Development Kit(SDK) for rapid development of microservices in Go
- [Java: Dubbo](http://dubbo.io/): DUBBO是一个分布式服务框架，致力于提供高性能和透明化的RPC远程服务调用方案，是阿里巴巴SOA服务化治理方案的核心框架，每天为2,000+个服务提供3,000,000,000+次访问量支持，并被广泛应用于阿里巴巴集团的各成员站点。
- [Java: Dubbox](https://github.com/dangdangdotcom/dubbox): Dubbox now means Dubbo eXtensions, and it adds features like RESTful remoting, Kyro/FST serialization, etc to the Dubbo service framework.
- [Java: Motan](https://github.com/weibocom/motan): A remote procedure call(RPC) framework for rapid development of high performance distributed services.
- [.NET: Zyan Communication Framework](http://zyan.com.de/): Easy to use distributed application framework for .NET, Mono and Xamarin.Android.
- [.NET: Akka.net](http://getakka.net/): a toolkit and runtime for building highly concurrent, distributed, and fault tolerant event-driven applications on .NET & Mono.

## Data Exchange Format

- [Portocol Buffer](https://developers.google.com/protocol-buffers/): Protocol buffers are Google's language-neutral, platform-neutral, extensible mechanism for serializing structured data – think XML, but smaller, faster, and simpler.
- [Message Pack](http://msgpack.org/): MessagePack is an efficient binary serialization format. It lets you exchange data among multiple languages like JSON. But it's faster and smaller. Small integers are encoded into a single byte, and typical short strings require only one extra byte in addition to the strings themselves.
- [Apache Thrift](http://thrift.apache.org/): Thrift源于大名鼎鼎的facebook之手，在2007年facebook提交Apache基金会将Thrift作为一个开源项目，对于当时的facebook来说创造thrift是为了解决facebook系统中各系统间大数据量的传输通信以及系统之间语言环境不同需要跨平台的特性。所以thrift可以支持多种程序语言，例如: C++, C#, Cocoa, Erlang Haskell, Java, Ocami, Perl, PHP, Python, Ruby, Smalltalk. 在多种不同的语言之间通信thrift可以作为二进制的高性能的通讯中间件，支持数据(对象)序列化和多种类型的RPC服务。Thrift适用于程序对程序静态的数据交换，需要先确定好他的数据结构，他是完全静态化的，当数据结构发生变化时，必须重新编辑IDL文件，代码生成，再编译载入的流程，跟其他IDL工具相比较可以视为是Thrift的弱项，Thrift适用于搭建大型数据交换及存储的通用工具，对于大型系统中的内部数据传输相对于JSON和xml无论在性能、传输大小上有明显的优势。
- [Apache Avro](http://avro.apache.org/): Apache Avro™ is a data serialization system.
- [Cap'n Proto](https://capnproto.org/index.html): Cap'n Proto is an insanely fast data interchange format and capability-based RPC system. Think JSON, except binary. Or think Protocol Buffers, except faster. In fact, in benchmarks, Cap'n Proto is INFINITY TIMES faster than Protocol Buffers.
- [Microsoft bond](https://github.com/Microsoft/bond): Bond is a cross-platform framework for working with schematized data. It supports cross-language de/serialization and powerful generic mechanisms for efficiently manipulating data. Bond is broadly used at Microsoft in high scale services.
- [JSON](http://json.org/): JSON (JavaScript Object Notation) is a lightweight data-interchange format. It is easy for humans to read and write. It is easy for machines to parse and generate. It is based on a subset of the JavaScript Programming Language, Standard ECMA-262 3rd Edition - December 1999\. JSON is a text format that is completely language independent but uses conventions that are familiar to programmers of the C-family of languages, including C, C++, C#, Java, JavaScript, Perl, Python, and many others. These properties make JSON an ideal data-interchange language.
  - [JSON Schema](http://json-schema.org/)
  - [JSON Schema Generator](http://jsonschema.net/)

## RPC

- [GRPC](http://www.grpc.io/): A high performance, open source, general RPC framework that puts mobile and HTTP/2 first.
  - [rpcx](https://github.com/smallnest/rpcx): A RPC service framework based on net/rpc like alibaba Dubbo and weibo Motan. One of best performance RPC frameworks.
- [Hprose](http://hprose.com/): 一款先进的轻量级、跨语言、跨平台、无侵入式、高性能动态远程对象调用引擎库
- [ZeroC](https://zeroc.com/): Ice is more than a RPC framework. It also provides a number of complementary services for your networked applications.
- [Finagle](https://twitter.github.io/finagle/): Finagle is an extensible RPC system for the JVM, used to construct high-concurrency servers. Finagle implements uniform client and server APIs for several protocols, and is designed for high performance and concurrency. Most of Finagle's code is protocol agnostic, simplifying the implementation of new protocols.
- [brpc](https://github.com/brpc/brpc): Most common RPC framework used throughout Baidu, with 600,000+ instances and 500+ kinds of services, called "baidu-rpc" inside Baidu.
- [tars](https://github.com/Tencent/Tars): Tars是腾讯从2008年到今天一直在使用的后台逻辑层的统一应用框架TAF（Total Application Framework），目前支持C++和Java两种语言。该框架为用户提供了涉及到开发、运维、以及测试的一整套解决方案，帮助一个产品或者服务快速开发、部署、测试、上线。 它集可扩展协议编解码、高性能RPC通信框架、名字路由与发现、发布监控、日志统计、配置管理等于一体，通过它可以快速用微服务的方式构建自己的稳定可靠的分布式应用，并实现完整有效的服务治理。

## Service Bus

- [Java: Apache Camel](http://camel.apache.org/): Apache Camel is a versatile open-source integration framework based on known Enterprise Integration Patterns. The following projects can leverage Apache Camel as a routing and mediation engine:
	- Apache ServiceMix
	- Apache ActiveMQ
	- Apache CXF
	- Apache Karaf
	- Apache MINA
- [Java: Spring Integration](http://projects.spring.io/spring-integration/): Extends the Spring programming model to support the well-known Enterprise Integration Patterns. Spring Integration enables lightweight messaging within Spring-based applications and supports integration with external systems via declarative adapters.
- [Java: Mule ESB community](https://github.com/mulesoft/mule): Mule Community Edition
- [.NET: MassTransit](http://masstransit-project.com/): Lean Service Bus for .NET
- [.NET: NServiceBus](https://github.com/Particular): The most popular service bus for .NET
- [.NET: Rebus](https://github.com/rebus-org/Rebus): Rebus is a lean service bus implementation for .NET, similar in nature to NServiceBus and MassTransit, only leaner
- [.NET: Shuttle-ESB](http://shuttle.github.io/shuttle-esb/): A highly configurable free open-source enterprise service bus that provides you with a mechanism to create Autonomous Business Components that are loosely coupled. This enables you to develop and deploy specific business functionality that can be independently versioned.

## Messsage Queue

- [C++: ZeroMQ](http://zeromq.org/): ZeroMQ (also known as ØMQ, 0MQ, or zmq) looks like an embeddable networking library but acts like a concurrency framework. It gives you sockets that carry atomic messages across various transports like in-process, inter-process, TCP, and multicast. You can connect sockets N-to-N with patterns like fan-out, pub-sub, task distribution, and request-reply. It's fast enough to be the fabric for clustered products. Its asynchronous I/O model gives you scalable multicore applications, built as asynchronous message-processing tasks. It has a score of language APIs and runs on most operating systems
    - [C#: NetMQ](https://github.com/zeromq/netmq): NetMQ is 100% native C# port of ZeroMQ
    - [Java: JeroMQ](https://github.com/zeromq/jeromq): Pure Java implementation of libzmq
- [C: beanstalkd](http://kr.github.io/beanstalkd/): Beanstalk is a simple, fast work queue. Its interface is generic, but was originally designed for reducing the latency of page views in high-volume web applications by running time-consuming tasks asynchronously.
- [Erlang: RabbitMQ](http://www.rabbitmq.com/): RabbitMQ is a messaging broker - an intermediary for messaging. It gives your applications a common platform to send and receive messages, and your messages a safe place to live until received.
    - [RabbitMQ Internals](https://github.com/rabbitmq/internals): This project aims to explain how RabbitMQ works internally. The goal is to make it easier to contribute for newcomers to the project, and at the same time have a common repository of knowledge to be shared across the project contributors.
- [Java: Apache Kafka](http://kafka.apache.org/): Apache Kafka is publish-subscribe messaging rethought as a distributed commit log.
  - [KSQL](https://github.com/confluentinc/ksql): a Streaming SQL Engine for Apache Kafka
  - [Kafka Manager](https://github.com/yahoo/kafka-manager): A tool for managing Apache Kafka
  - [confluent](https://www.confluent.io/product/confluent-open-source/): A developer-optimized distribution of Apache Kafka
- [Java: RocketMQ](https://rocketmq.apache.org/): Apache RocketMQ™ is an open source distributed messaging and streaming data platform.
- [Java: Apache ActiveMQ](http://activemq.apache.org/): Apache ActiveMQ ™ is the most popular and powerful open source messaging and Integration Patterns server. Apache ActiveMQ is fast, supports many Cross Language Clients and Protocols, comes with easy to use Enterprise Integration Patterns and many advanced features while fully supporting JMS 1.1 and J2EE 1.4\. Apache ActiveMQ is released under the Apache 2.0 License.
- [Go: NATS](https://nats.io/): NATS is an open-source, cloud-native messaging system. In addition to functioning as the “nervous system” for the Apcera platform, companies like Baidu, Siemens, VMware, HTC, and Ericsson rely on NATS for its highly performant and resilient messaging capabilities.
- [Go: NSQ](https://github.com/bitly/nsq): NSQ is a realtime distributed messaging platform designed to operate at scale, handling billions of messages per day.
- [Go: rmq](https://github.com/adjust/rmq): rmq is short for Redis message queue. It's a message queue system written in Go and backed by Redis. It's similar to redismq, but implemented independently with a different interface in mind.
- [Node: kue](https://github.com/Automattic/kue): Kue is a priority job queue backed by redis, built for node.js.

## Job Schedule

- [Java: elastic-job](https://github.com/dangdangdotcom/elastic-job): Elastic-Job is a distributed scheduled job framework, based on Quartz and Zookeeper.
- [Java: Saturn](https://github.com/vipshop/Saturn)
- [Java: Quartz](http://quartz-scheduler.org/): Quartz is a richly featured, open source job scheduling library that can be integrated within virtually any Java application - from the smallest stand-alone application to the largest e-commerce system. Quartz can be used to create simple or complex schedules for executing tens, hundreds, or even tens-of-thousands of jobs; jobs whose tasks are defined as standard Java components that may execute virtually anything you may program them to do. The Quartz Scheduler includes many enterprise-class features, such as support for JTA transactions and clustering.
- [Java: Airflow](https://github.com/airbnb/airflow): a workflow management platform
- [Java: rundeck](http://rundeck.org/index.html): job scheduler and runbook automation
- [Java: schedulix - open source enterprise job scheduling](https://github.com/schedulix/schedulix): schedulix is an open source enterprise job scheduling system.
- [Java: Azkaban](https://azkaban.github.io/): Azkaban is a batch workflow job scheduler created at LinkedIn to run Hadoop jobs. Azkaban resolves the ordering through job dependencies and provides an easy to use web user interface to maintain and track your workflows.
- [C#: Quartz.Net](https://github.com/quartznet/quartznet): Quartz.NET is a pure .NET library written in C# and is a port of very popular open source Java job scheduling framework, Quartz.
- [C#: FluentScheduler](https://github.com/jgeurts/FluentScheduler): A task scheduler that uses fluent interface to configure schedules. Useful for running cron jobs/automated tasks from your application.
- [C#: Hangfire](https://github.com/HangfireIO/Hangfire): Incredibly easy way to perform fire-and-forget, delayed and recurring tasks inside ASP.NET applications
- [C: Gearman](http://gearman.org/): Gearman provides a generic application framework to farm out work to other machines or processes that are better suited to do the work. It allows you to do work in parallel, to load balance processing, and to call functions between languages. It can be used in a variety of applications, from high-availability web sites to the transport of database replication events.
- [Ruby: resque-schedule](https://github.com/resque/resque-scheduler): A light-weight job scheduling system built on top of resque
- [Python: celery](http://www.celeryproject.org/): Celery is an asynchronous task queue/job queue based on distributed message passing.	It is focused on real-time operation, but supports scheduling as well.
- [Python: luigi](https://github.com/spotify/luigi): Luigi is a Python module that helps you build complex pipelines of batch jobs. It handles dependency resolution, workflow management, visualization etc. It also comes with Hadoop support built in.
- [Python: pinball](https://github.com/pinterest/pinball): Pinball is a scalable workflow manager
- [Go: kala](https://github.com/ajvb/kala): Kala is a simplistic, modern, and performant job scheduler written in Go. It lives in a single binary and does not have any dependencies. (Currently in Alpha stage. Do not use in production environments.)
- [Go: dkron](https://github.com/victorcoder/dkron): Distributed, fault tolerant job scheduling system
- [Go: jobber](https://github.com/dshearer/jobber): A replacement for cron, with sophisticated status-reporting and error-handling.
- [Go: cron](https://github.com/robfig/cron): a cron library for go
- [Go: gocron](https://github.com/jasonlvhit/gocron): A Golang Job Scheduling Package.
- [Go: scheduler](https://github.com/carlescere/scheduler): Job scheduling made easy.
- [Go: workq](https://github.com/iamduo/workq): Workq is a job scheduling server strictly focused on simplifying job processing and streamlining coordination. It can run jobs in blocking foreground or non-blocking background mode.
- [Go: cronsun](https://github.com/shunfei/cronsun): A Distributed, Fault-Tolerant Cron-Style Job System.
- [Go: goworker](https://github.com/benmanns/goworker): goworker is a Go-based background worker that runs 10 to 100,000* times faster than Ruby-based workers.
- [Go: machinery](https://github.com/RichardKnop/machinery): Machinery is an asynchronous task queue/job queue based on distributed message passing.
- [Go: fireworq](https://github.com/fireworq/fireworq): Fireworq is a lightweight, high-performance, language-independent job queue system.

## Load Balance

- [Nginx](http://wiki.nginx.org/Main): Nginx (pronounced engine-x) is a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
- [LVS](http://www.linuxvirtualserver.org/): The Linux Virtual Server is a highly scalable and highly available server built on a cluster of real servers, with the load balancer running on the Linux operating system. The architecture of the server cluster is fully transparent to end users, and the users interact as if it were a single high-performance virtual server.
- [HAProxy](http://www.haproxy.org/): HAProxy is a free, very fast and reliable solution offering high availability, load balancing, and proxying for TCP and HTTP-based applications.
  - [Bamboo](https://github.com/QubitProducts/bamboo): HAProxy auto configuration and auto service discovery for Mesos Marathon
- [keepalived](http://www.keepalived.org/): Keepalived is a routing software written in C. The main goal of this project is to provide simple and robust facilities for loadbalancing and high-availability to Linux system and Linux based infrastructures.
- [Go: Seesaw](https://github.com/google/seesaw): Seesaw v2 is a Linux Virtual Server (LVS) based load balancing platform.
- [Pen](http://siag.nu/pen/): Pen is a load balancer for "simple" TCP-based protocols such as HTTP or SMTP. It allows several servers to appear as one to the outside. It automatically detects servers that are down and distributes clients among the available servers. This gives high availability and scalable performance.
- [Balance](http://www.inlab.de/balance.html): Balance is a simple but powerful generic TCP proxy with round-robin load balancing and failover mechanisms. Its behavior can be controlled at runtime using a simple command line syntax. Balance supports IPv6 on the listening side, which makes it a very useful tool for IPv6 migration of IPv4 only services and servers.

## API Gateway

- [C: Nginx](https://github.com/nginx/nginx): a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
  - [Nginx Wiki](http://wiki.nginx.org/Main)
  - [C: OpenResty](https://openresty.org/cn/): OpenResty ™ 是一个基于 Nginx 与 Lua 的高性能 Web 平台，其内部集成了大量精良的 Lua 库、第三方模块以及大多数的依赖项。用于方便地搭建能够处理超高并发、扩展性极高的动态 Web 应用、Web 服务和动态网关。
  - [Lua: Kong](https://github.com/Mashape/kong): Open-source, Microservice & API Management Layer built on top of NGINX
- [Go: Caddy](https://github.com/mholt/caddy): Fast, cross-platform HTTP/2 web server with automatic HTTPS
- [Go: Tyk API Gateway](https://github.com/lonelycode/tyk): Tyk is a lightweight, open source API Gateway and enables you to control who accesses your API, when they access it and how they access it. Tyk will also record detailed analytics on how your users are interacting with your API and when things go wrong.
    - [Documents](https://tyk.io/tyk-documentation/concepts/)
- [Go: KrakenD](http://www.krakend.io/): KrakenD aggregates and manipulates multiple data sources to provide you with exactly the API your end-user products need while offering a premium user experience and brutal performance.

## API Proxy

- [C++: Envoy](https://github.com/lyft/envoy): C++ L7 proxy and communication bus
- [Scala: linkerd](https://linkerd.io/): Modern RPC proxy for microservices

## Reverse Proxy

- [Nginx](http://wiki.nginx.org/Main): Nginx (pronounced engine-x) is a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
- [Traefik](https://github.com/containous/traefik/): Træfik (pronounced like traffic) is a modern HTTP reverse proxy and load balancer made to deploy microservices with ease. It supports several backends (Docker, Swarm mode, Kubernetes, Marathon, Consul, Etcd, Rancher, Amazon ECS, and a lot more) to manage its configuration automatically and dynamically.
- [Varnish](https://www.varnish-cache.org/): Varnish是一款高性能且开源的反向代理服务器和http加速器。与传统的Squid相比，Varnish具有性能更高、速度更快、管理更方便 等诸多优点。作者Poul-Henning Kamp是FreeBSD的内核开发者之一。Varnish采用全新的软件体系架构，和现在的硬件提交配合紧密。在1975年时，储存媒介只有两种：内存 与硬盘。但现在计算 机系统的内存除了主存外，还包括了cpu内的L1、L2，甚至有L3快取。硬盘上也有自己的快取装置，因此squid cache自行处理物件替换的架构不可能得知这些情况而做到最佳化，但操作系统可以得知这些情况，所以这部份的工作应该交给操作系统处理，这就是 Varnish cache设计架构。挪威最大的在线报纸Verdens Gang使用3台Varnish代替了原来的12台squid，性能居然比以前更好，这是Varnish最成功的应用案例。
- [Squid](http://www.squid-cache.org/): Squid is a caching proxy for the Web supporting HTTP, HTTPS, FTP, and more. It reduces bandwidth and improves response times by caching and reusing frequently-requested web pages. Squid has extensive access controls and makes a great server accelerator. It runs on most available operating systems, including Windows and is licensed under the GNU GPL.

## Distributed File System

- [Ceph](http://ceph.com/): Ceph is a distributed object store and file system designed to provide excellent performance, reliability and scalability. See more at: <http://ceph.com/#sthash.46aGKE2z.dpuf>
- [MooseFS](http://www.moosefs.org/): MooseFS is a fault tolerant, network distributed file system. It spreads data over several physical servers which are visible to the user as one resource.
- [Glusterfs](http://www.gluster.org/): GlusterFS is a scalable network filesystem. Using common off-the-shelf hardware, you can create large, distributed storage solutions for media streaming, data analysis, and other data- and bandwidth-intensive tasks. GlusterFS is free and open source software.
- [FastDFS](https://code.google.com/p/fastdfs/): [FastDFS on Google Code](https://code.google.com/p/fastdfs/), FastDFS is an open source high performance distributed file system. It's major functions include: file storing, file syncing and file accessing, and design for high capacity and load balance.
- [mogilefs](https://github.com/mogilefs/): MogileFS is our open source distributed filesystem.
- [XtreeFS](http://xtreemfs.org/index.php): XtreemFS is a general purpose storage system and covers most storage needs in a single deployment. It is open-source, requires no special hardware or kernel modules, and can be mounted on Linux, Windows and OS X.
- [Taobao File System](http://tfs.taobao.org/): TFS（Taobao !FileSystem）是一个高可扩展、高可用、高性能、面向互联网服务的分布式文件系统，主要针对海量的非结构化数据，它构筑在普通的Linux机器集群上，可为外部提供高可靠和高并发的存储访问。TFS为淘宝提供海量小文件存储，通常文件大小不超过1M，满足了淘宝对小文件存储的需求，被广泛地应用在淘宝各项应用中。它采用了HA架构和平滑扩容，保证了整个文件系统的可用性和扩展性。同时扁平化的数据组织结构，可将文件名映射到文件的物理地址，简化了文件的访问流程，一定程度上为TFS提供了良好的读写性能。
- [seaweedfs](https://github.com/chrislusf/seaweedfs): Seaweed-FS is a simple and highly scalable distributed file system. There are two objectives: to store billions of files! to serve the files fast! Instead of supporting full POSIX file system semantics, Seaweed-FS choose to implement only a key~file mapping. Similar to the word "NoSQL", you can call it as "NoFS".
- [GlusterFS](http://www.gluster.org/): GlusterFS is a scalable network filesystem. Using common off-the-shelf hardware, you can create large, distributed storage solutions for media streaming, data analysis, and other data- and bandwidth-intensive tasks. GlusterFS is free and open source software.
- [BeeGFS](http://www.beegfs.com/content/): BeeGFS (formerly FhGFS) is the leading parallel cluster file system, developed with a strong focus on performance and designed for very easy installation and management. If I/O intensive workloads are your problem, BeeGFS is the solution.

## Configuration Management

- [Confd](https://github.com/kelseyhightower/confd): Manage local application configuration files using templates and data from etcd or consul
- [Consul Template](https://github.com/hashicorp/consul-template): This project provides a convenient way to populate values from Consul into the filesystem using the consul-template daemon. Consul into the filesystem using the consul-template daemon.
- [disconf](https://github.com/knightliao/disconf): Distributed Configuration Management Platform(分布式配置管理平台)
- [Qconf](https://github.com/Qihoo360/QConf): Qihoo Distrubuted Configuration Management System
- [super diamond](https://github.com/melin/super-diamond): 配置管理系统
- [XDiamond](https://github.com/hengyunabc/xdiamond): 全局配置中心，存储应用的配置项，解决配置混乱分散的问题。名字来源于淘宝的开源项目diamond，前面加上一个字母X以示区别。
- [archaius](https://github.com/Netflix/archaius): Library for configuration management API

## Service Discovery, Name Service

- [Apache Zookeeper](http://zookeeper.apache.org/): ZooKeeper is a centralized service for maintaining configuration information, naming, providing distributed synchronization, and providing group services. All of these kinds of services are used in some form or another by distributed applications. Each time they are implemented there is a lot of work that goes into fixing the bugs and race conditions that are inevitable. Because of the difficulty of implementing these kinds of services, applications initially usually skimp on them ,which make them brittle in the presence of change and difficult to manage. Even when done correctly, different implementations of these services lead to management complexity when the applications are deployed.Application tracing system for Go, based on Google's Dapper.
- [etcd](https://github.com/coreos/etcd): A distributed consistent key-value store for shared configuration and service discovery
- [consul](https://www.consul.io/): Consul 简化了分布式环境中的服务的注册和发现流程，通过 HTTP 或者 DNS 接口发现。支持外部 SaaS 提供者等
- [serf](https://github.com/hashicorp/serf): Service orchestration and management tool

## DNS Server

- [Dnsmasq](http://www.thekelleys.org.uk/dnsmasq/doc.html): Dnsmasq provides network infrastructure for small networks: DNS, DHCP, router advertisement and network boot. It is designed to be lightweight and have a small footprint, suitable for resource constrained routers and firewalls. It has also been widely used for tethering on smartphones and portable hotspots, and to support virtual networking in virtualisation frameworks.
- [PowerDNS](https://github.com/PowerDNS/pdns): There are two PowerDNS nameserver products: the Authoritative Server and the Recursor. While most other nameservers fully combine these functions, PowerDNS offers them separately, but can mix both authoritative and recursive usage seamlessly.
- [SkyDNS](https://github.com/skynetservices/skydns): SkyDNS is a distributed service for announcement and discovery of services built on top of etcd. It utilizes DNS queries to discover available services. This is done by leveraging SRV records in DNS, with special meaning given to subdomains, priorities and weights.

## Circuit Breaker

- [Go: Hystrix-go](https://github.com/afex/hystrix-go): Netflix's Hystrix latency and fault tolerance library, for Go
- [Go: gobreaker](https://github.com/sony/gobreaker): Circuit Breaker implemented in Go
- [Java: Hystrix](https://github.com/Netflix/Hystrix): Hystrix is a latency and fault tolerance library designed to isolate points of access to remote systems, services and 3rd party libraries, stop cascading failure and enable resilience in complex distributed systems where failure is inevitable.
- [C#: Polly](https://github.com/App-vNext/Polly): Polly is a .NET 3.5 / 4.0 / 4.5 / PCL library that allows developers to express transient exception handling policies such as Retry, Retry Forever, Wait and Retry or Circuit Breaker in a fluent manner.
- [C#: Hystrix.NET](https://hystrixnet.codeplex.com): Hystrix.NET is a C# port of Hystrix, which is a latency and fault tolerance library for complex distributed systems.


## Distributed Tracing

- [Open Tracing](http://opentracing.io/): Consistent, expressive, vendor-neutral APIs for distributed tracing and context propagation
- [AppDash](https://github.com/sourcegraph/appdash): Application tracing system for Go, based on Google's Dapper.
- [zipkin](https://github.com/openzipkin/zipkin): Zipkin is a distributed tracing system
- [Jaeger](https://github.com/uber/jaeger): Jaeger, a Distributed Tracing System
  - [Jaeger-client-go](https://github.com/uber/jaeger-client-go): Jaeger Bindings for Go OpenTracing API.

## Other

- [Golang: Sonyflake](https://github.com/sony/sonyflake): A distributed unique ID generator inspired by Twitter's Snowflake
