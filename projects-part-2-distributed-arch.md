- [Projects about Distributed Architecture](#projects-about-distributed-architecture)
  - [Open Platform](#open-platform)
  - [Distributed Application Framework](#distributed-application-framework)
  - [Data Exchange Format](#data-exchange-format)
  - [RPC](#rpc)
  - [Service Bus](#service-bus)
  - [Message Queue](#message-queue)
  - [Job Schedule](#job-schedule)
  - [Load Balance](#load-balance)
  - [API Gateway && API Proxy](#api-gateway--api-proxy)
  - [GraphQL](#graphql)
  - [Reverse Proxy](#reverse-proxy)
  - [Distributed File System](#distributed-file-system)
  - [Configuration Management](#configuration-management)
  - [Service Discovery, Name Service](#service-discovery-name-service)
  - [DNS Server](#dns-server)
  - [Circuit Breaker](#circuit-breaker)
  - [Distributed Tracing](#distributed-tracing)
  - [Cache](#cache)
  - [Database Driver](#database-driver)
  - [Other](#other)


# Projects about Distributed Architecture

## Open Platform

- [Istio](https://istio.io/): An open platform to connect, manage, and secure microservices

## Distributed Application Framework

- [Go: go-kit](https://github.com/go-kit): A standard library for microservices.
- [Go: micro](https://github.com/micro): A microservice toolkit for distributed systems development
- [Go: go-chassis](https://github.com/ServiceComb): Go-Chassis is a Software Development Kit(SDK) for rapid development of microservices in Go
- [Java: Dubbo](http://dubbo.apache.org/): DUBBO是一个分布式服务框架，致力于提供高性能和透明化的RPC远程服务调用方案，是阿里巴巴SOA服务化治理方案的核心框架，每天为2,000+个服务提供3,000,000,000+次访问量支持，并被广泛应用于阿里巴巴集团的各成员站点。
- [Java: Dubbox](https://github.com/dangdangdotcom/dubbox): Dubbox now means Dubbo eXtensions, and it adds features like RESTful remoting, Kyro/FST serialization, etc to the Dubbo service framework.
- [Java: Motan](https://github.com/weibocom/motan): A remote procedure call(RPC) framework for rapid development of high performance distributed services.
- [.NET: Zyan Communication Framework](http://zyan.com.de/): Easy to use distributed application framework for .NET, Mono and Xamarin.Android.
- [.NET: Akka.net](http://getakka.net/): a toolkit and runtime for building highly concurrent, distributed, and fault tolerant event-driven applications on .NET & Mono.

## Data Exchange Format

- [Protocol Buffers](https://developers.google.com/protocol-buffers/): Protocol buffers are Google's language-neutral, platform-neutral, extensible mechanism for serializing structured data – think XML, but smaller, faster, and simpler.
- [Message Pack](http://msgpack.org/): MessagePack is an efficient binary serialization format. It lets you exchange data among multiple languages like JSON. But it's faster and smaller. Small integers are encoded into a single byte, and typical short strings require only one extra byte in addition to the strings themselves.
- [Apache Thrift](http://thrift.apache.org/): Thrift源于大名鼎鼎的facebook之手，在2007年facebook提交Apache基金会将Thrift作为一个开源项目，对于当时的facebook来说创造thrift是为了解决facebook系统中各系统间大数据量的传输通信以及系统之间语言环境不同需要跨平台的特性。所以thrift可以支持多种程序语言，例如: C++, C#, Cocoa, Erlang Haskell, Java, Ocami, Perl, PHP, Python, Ruby, Smalltalk. 在多种不同的语言之间通信thrift可以作为二进制的高性能的通讯中间件，支持数据(对象)序列化和多种类型的RPC服务。Thrift适用于程序对程序静态的数据交换，需要先确定好他的数据结构，他是完全静态化的，当数据结构发生变化时，必须重新编辑IDL文件，代码生成，再编译载入的流程，跟其他IDL工具相比较可以视为是Thrift的弱项，Thrift适用于搭建大型数据交换及存储的通用工具，对于大型系统中的内部数据传输相对于JSON和xml无论在性能、传输大小上有明显的优势。
- [Apache Avro](http://avro.apache.org/): Apache Avro™ is a data serialization system.
- [Cap'n Proto](https://capnproto.org/index.html): Cap'n Proto is an insanely fast data interchange format and capability-based RPC system. Think JSON, except binary. Or think Protocol Buffers, except faster. In fact, in benchmarks, Cap'n Proto is INFINITY TIMES faster than Protocol Buffers.
- [Microsoft bond](https://github.com/Microsoft/bond): Bond is a cross-platform framework for working with schematized data. It supports cross-language de/serialization and powerful generic mechanisms for efficiently manipulating data. Bond is broadly used at Microsoft in high scale services.
- [JSON](http://json.org/): JSON (JavaScript Object Notation) is a lightweight data-interchange format. It is easy for humans to read and write. It is easy for machines to parse and generate. It is based on a subset of the JavaScript Programming Language, Standard ECMA-262 3rd Edition - December 1999\. JSON is a text format that is completely language independent but uses conventions that are familiar to programmers of the C-family of languages, including C, C++, C#, Java, JavaScript, Perl, Python, and many others. These properties make JSON an ideal data-interchange language.
  - [JSON Schema](http://json-schema.org/)
  - [JSON Schema Generator](http://jsonschema.net/)
- [Apache Arrow](https://arrow.apache.org/): A cross-language development platform for in-memory analytics

## RPC

- [GRPC](http://www.grpc.io/): A high performance, open source, general RPC framework that puts mobile and HTTP/2 first.
  - [rpcx](https://github.com/smallnest/rpcx): A RPC service framework based on net/rpc like alibaba Dubbo and weibo Motan. One of best performance RPC frameworks.
- [Hprose](http://hprose.com/): 一款先进的轻量级、跨语言、跨平台、无侵入式、高性能动态远程对象调用引擎库
- [ZeroC](https://zeroc.com/): Ice is more than a RPC framework. It also provides a number of complementary services for your networked applications.
- [Finagle](https://twitter.github.io/finagle/): Finagle is an extensible RPC system for the JVM, used to construct high-concurrency servers. Finagle implements uniform client and server APIs for several protocols, and is designed for high performance and concurrency. Most of Finagle's code is protocol agnostic, simplifying the implementation of new protocols.
- [brpc](https://github.com/brpc/brpc): Most common RPC framework used throughout Baidu, with 600,000+ instances and 500+ kinds of services, called "baidu-rpc" inside Baidu.
- [tars](https://github.com/Tencent/Tars): Tars是腾讯从2008年到今天一直在使用的后台逻辑层的统一应用框架TAF（Total Application Framework），目前支持C++和Java两种语言。该框架为用户提供了涉及到开发、运维、以及测试的一整套解决方案，帮助一个产品或者服务快速开发、部署、测试、上线。 它集可扩展协议编解码、高性能RPC通信框架、名字路由与发现、发布监控、日志统计、配置管理等于一体，通过它可以快速用微服务的方式构建自己的稳定可靠的分布式应用，并实现完整有效的服务治理。
- [sofa-pbrpc](https://github.com/baidu/sofa-pbrpc): A light-weight RPC implementation of Google's protobuf RPC framework.


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

## Message Queue

- [C++: ZeroMQ](http://zeromq.org/): ZeroMQ (also known as ØMQ, 0MQ, or zmq) looks like an embeddable networking library but acts like a concurrency framework. It gives you sockets that carry atomic messages across various transports like in-process, inter-process, TCP, and multicast. You can connect sockets N-to-N with patterns like fan-out, pub-sub, task distribution, and request-reply. It's fast enough to be the fabric for clustered products. Its asynchronous I/O model gives you scalable multicore applications, built as asynchronous message-processing tasks. It has a score of language APIs and runs on most operating systems
    - [C#: NetMQ](https://github.com/zeromq/netmq): NetMQ is 100% native C# port of ZeroMQ
    - [Java: JeroMQ](https://github.com/zeromq/jeromq): Pure Java implementation of libzmq
- [C: beanstalkd](http://kr.github.io/beanstalkd/): Beanstalk is a simple, fast work queue. Its interface is generic, but was originally designed for reducing the latency of page views in high-volume web applications by running time-consuming tasks asynchronously.
- [C: Gearman](http://gearman.org/): Gearman provides a generic application framework to farm out work to other machines or processes that are better suited to do the work. It allows you to do work in parallel, to load balance processing, and to call functions between languages. It can be used in a variety of applications, from high-availability web sites to the transport of database replication events.
- [Erlang: RabbitMQ](http://www.rabbitmq.com/): RabbitMQ is a messaging broker - an intermediary for messaging. It gives your applications a common platform to send and receive messages, and your messages a safe place to live until received.
    - [RabbitMQ Internals](https://github.com/rabbitmq/internals): This project aims to explain how RabbitMQ works internally. The goal is to make it easier to contribute for newcomers to the project, and at the same time have a common repository of knowledge to be shared across the project contributors.
- [Java: Apache Kafka](http://kafka.apache.org/): Apache Kafka is publish-subscribe messaging rethought as a distributed commit log.
  - [KSQL](https://github.com/confluentinc/ksql): a Streaming SQL Engine for Apache Kafka
  - [Kafka Manager](https://github.com/yahoo/kafka-manager): A tool for managing Apache Kafka
  - [confluent](https://www.confluent.io/product/confluent-open-source/): A developer-optimized distribution of Apache Kafka
  - [Kafka Center](https://github.com/xaecbd/KafkaCenter): KafkaCenter is a unified one-stop platform for Kafka cluster management and maintenance, producer / consumer monitoring, and use of ecological components.
- [Java: RocketMQ](https://rocketmq.apache.org/): Apache RocketMQ™ is an open source distributed messaging and streaming data platform.
- [Java: ActiveMQ](http://activemq.apache.org/): Apache ActiveMQ ™ is the most popular and powerful open source messaging and Integration Patterns server. Apache ActiveMQ is fast, supports many Cross Language Clients and Protocols, comes with easy to use Enterprise Integration Patterns and many advanced features while fully supporting JMS 1.1 and J2EE 1.4\. Apache ActiveMQ is released under the Apache 2.0 License.
- [Java: Apache Pulsar](https://pulsar.apache.org/en/): Pulsar is a distributed pub-sub messaging platform with a very flexible messaging model and an intuitive client API.
- [Go: NATS](https://nats.io/): NATS is an open-source, cloud-native messaging system. In addition to functioning as the “nervous system” for the Apcera platform, companies like Baidu, Siemens, VMware, HTC, and Ericsson rely on NATS for its highly performant and resilient messaging capabilities.
- [Go: NSQ](https://github.com/bitly/nsq): NSQ is a realtime distributed messaging platform designed to operate at scale, handling billions of messages per day.
- [Go: rmq](https://github.com/adjust/rmq): rmq is short for Redis message queue. It's a message queue system written in Go and backed by Redis. It's similar to redismq, but implemented independently with a different interface in mind.
- [Node: kue](https://github.com/Automattic/kue): Kue is a priority job queue backed by redis, built for node.js.

Open Messaging:

- [OpenMessaging](http://openmessaging.cloud/): Messaging and Streaming products have been widely used in modern architecture and data processing, for decoupling, queuing, buffering, ordering, replicating, etc. But when data transfers across different messaging and streaming platforms, the compatibility problem arises, which always means much additional work. Although JMS was a good solution during the past decade, it is limited in java environment, lacks specified guidelines for load balance/fault-tolerance, administration, security, and streaming feature, which make it not good at satisfying modern cloud-oriented messaging and streaming applications.
  - [解读OpenMessaging开源项目，阿里巴巴发起首个分布式消息领域的国际标准](http://jm.taobao.org/2017/10/18/20171018/)
  - [OPENMESSAGING DOMAIN ARCHITECTURE](http://openmessaging.cloud/design/2018/03/28/openmessaging-domain-architecture-v0.3/)

## Job Schedule

- [Java: elastic-job](https://github.com/dangdangdotcom/elastic-job): Elastic-Job is a distributed scheduled job framework, based on Quartz and Zookeeper.
- [Java: Saturn](https://github.com/vipshop/Saturn)
- [Java: Quartz](http://quartz-scheduler.org/): Quartz is a richly featured, open source job scheduling library that can be integrated within virtually any Java application - from the smallest stand-alone application to the largest e-commerce system. Quartz can be used to create simple or complex schedules for executing tens, hundreds, or even tens-of-thousands of jobs; jobs whose tasks are defined as standard Java components that may execute virtually anything you may program them to do. The Quartz Scheduler includes many enterprise-class features, such as support for JTA transactions and clustering.
  - [C#: Quartz.Net](https://github.com/quartznet/quartznet): Quartz.NET is a pure .NET library written in C# and is a port of very popular open source Java job scheduling framework, Quartz.
- [Java: rundeck](http://rundeck.org/index.html): job scheduler and runbook automation
- [Java: schedulix - open source enterprise job scheduling](https://github.com/schedulix/schedulix): schedulix is an open source enterprise job scheduling system.
- [Java: DolphinScheduler](https://github.com/apache/dolphinscheduler): DolphinScheduler is a distributed and extensible workflow scheduler platform with powerful DAG visual interfaces, dedicated to solving complex job dependencies in the data pipeline and providing various types of jobs available out of the box.
- [Java: XXL-job](https://github.com/xuxueli/xxl-job): XXL-JOB是一个分布式任务调度平台
  - [XXL开源社区](https://www.xuxueli.com/index.html)
- [C#: FluentScheduler](https://github.com/jgeurts/FluentScheduler): A task scheduler that uses fluent interface to configure schedules. Useful for running cron jobs/automated tasks from your application.
- [C#: Hangfire](https://github.com/HangfireIO/Hangfire): Incredibly easy way to perform fire-and-forget, delayed and recurring tasks inside ASP.NET applications
- [Ruby: resque-schedule](https://github.com/resque/resque-scheduler): A light-weight job scheduling system built on top of resque
  - [Ruby: resque](https://github.com/resque/resque): Resque (pronounced like "rescue") is a Redis-backed library for creating background jobs, placing those jobs on multiple queues, and processing them later.
- [Python: celery](http://www.celeryproject.org/): Celery is an asynchronous task queue/job queue based on distributed message passing.	It is focused on real-time operation, but supports scheduling as well.
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
- [node: cronicle](https://github.com/jhuckaby/Cronicle): A simple, distributed task scheduler and runner with a web based UI.
- [Scala: Chronos](http://mesos.github.io/chronos/): Chronos is Airbnb's replacement for cron. It is a distributed and fault-tolerant scheduler that runs on top of Apache Mesos that can be used for job orchestration. It supports custom Mesos executors as well as the default command executor. Thus by default, Chronos executes sh (on most systems bash) scripts.
- [C++: Bistro](https://facebook.github.io/bistro/): A toolkit for making services that schedule and execute tasks.

## Load Balance

- [Nginx](http://wiki.nginx.org/Main): Nginx (pronounced engine-x) is a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
- [LVS](http://www.linuxvirtualserver.org/): The Linux Virtual Server is a highly scalable and highly available server built on a cluster of real servers, with the load balancer running on the Linux operating system. The architecture of the server cluster is fully transparent to end users, and the users interact as if it were a single high-performance virtual server.
- [HAProxy](http://www.haproxy.org/): HAProxy is a free, very fast and reliable solution offering high availability, load balancing, and proxying for TCP and HTTP-based applications.
  - [Bamboo](https://github.com/QubitProducts/bamboo): HAProxy auto configuration and auto service discovery for Mesos Marathon
- [keepalived](http://www.keepalived.org/): Keepalived is a routing software written in C. The main goal of this project is to provide simple and robust facilities for loadbalancing and high-availability to Linux system and Linux based infrastructures.
- [GLB](https://github.com/github/glb-director): The GitHub Load Balancer (GLB) Director is a set of components that provide a scalable set of stateless Layer 4 load balancer servers capable of line rate packet processing in bare metal datacenter environments, and is used in production to serve all traffic from GitHub's datacenters.
- [DPVS](https://github.com/iqiyi/dpvs): DPVS is a high performance Layer-4 load balancer based on DPDK. It's derived from Linux Virtual Server LVS and its modification alibaba/LVS.

- [Go: Seesaw](https://github.com/google/seesaw): Seesaw v2 is a Linux Virtual Server (LVS) based load balancing platform.

- [Balance](http://www.inlab.de/balance.html): Balance is a simple but powerful generic TCP proxy with round-robin load balancing and failover mechanisms. Its behavior can be controlled at runtime using a simple command line syntax. Balance supports IPv6 on the listening side, which makes it a very useful tool for IPv6 migration of IPv4 only services and servers.
- [Pen](http://siag.nu/pen/): Pen is a load balancer for "simple" TCP-based protocols such as HTTP or SMTP. It allows several servers to appear as one to the outside. It automatically detects servers that are down and distributes clients among the available servers. This gives high availability and scalable performance.

## API Gateway && API Proxy

API gateway:

- [C: Nginx](https://github.com/nginx/nginx): a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
  - [Nginx Wiki](http://wiki.nginx.org/Main)
  - [C: OpenResty](https://openresty.org/cn/): OpenResty ™ 是一个基于 Nginx 与 Lua 的高性能 Web 平台，其内部集成了大量精良的 Lua 库、第三方模块以及大多数的依赖项。用于方便地搭建能够处理超高并发、扩展性极高的动态 Web 应用、Web 服务和动态网关。
  - [Lua: Kong](https://github.com/Mashape/kong): Open-source, Microservice & API Management Layer built on top of NGINX
- [Go: Caddy](https://github.com/mholt/caddy): Fast, cross-platform HTTP/2 web server with automatic HTTPS
- [Go: Tyk API Gateway](https://github.com/lonelycode/tyk): Tyk is a lightweight, open source API Gateway and enables you to control who accesses your API, when they access it and how they access it. Tyk will also record detailed analytics on how your users are interacting with your API and when things go wrong.
    - [Documents](https://tyk.io/tyk-documentation/concepts/)
- [Go: KrakenD](http://www.krakend.io/): KrakenD aggregates and manipulates multiple data sources to provide you with exactly the API your end-user products need while offering a premium user experience and brutal performance.

API Proxy:

- [C++: Envoy](https://github.com/lyft/envoy): C++ L7 proxy and communication bus
- [Scala: linkerd](https://linkerd.io/): Modern RPC proxy for microservices

## GraphQL

- [Apollo GraphQL](https://www.apollographql.com/): Do GraphQL Right

## Reverse Proxy

- [Nginx](http://wiki.nginx.org/Main): Nginx (pronounced engine-x) is a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
- [Traefik](https://github.com/containous/traefik/): Træfik (pronounced like traffic) is a modern HTTP reverse proxy and load balancer made to deploy microservices with ease. It supports several backends (Docker, Swarm mode, Kubernetes, Marathon, Consul, Etcd, Rancher, Amazon ECS, and a lot more) to manage its configuration automatically and dynamically.
- [Varnish](https://www.varnish-cache.org/): Varnish是一款高性能且开源的反向代理服务器和http加速器。与传统的Squid相比，Varnish具有性能更高、速度更快、管理更方便 等诸多优点。作者Poul-Henning Kamp是FreeBSD的内核开发者之一。Varnish采用全新的软件体系架构，和现在的硬件提交配合紧密。在1975年时，储存媒介只有两种：内存 与硬盘。但现在计算 机系统的内存除了主存外，还包括了cpu内的L1、L2，甚至有L3快取。硬盘上也有自己的快取装置，因此squid cache自行处理物件替换的架构不可能得知这些情况而做到最佳化，但操作系统可以得知这些情况，所以这部份的工作应该交给操作系统处理，这就是 Varnish cache设计架构。挪威最大的在线报纸Verdens Gang使用3台Varnish代替了原来的12台squid，性能居然比以前更好，这是Varnish最成功的应用案例。
- [Squid](http://www.squid-cache.org/): Squid is a caching proxy for the Web supporting HTTP, HTTPS, FTP, and more. It reduces bandwidth and improves response times by caching and reusing frequently-requested web pages. Squid has extensive access controls and makes a great server accelerator. It runs on most available operating systems, including Windows and is licensed under the GNU GPL.

## Distributed File System

- [Ceph](http://ceph.com/): Ceph is a distributed object store and file system designed to provide excellent performance, reliability and scalability. See more at: <http://ceph.com/#sthash.46aGKE2z.dpuf>
- [Glusterfs](http://www.gluster.org/): GlusterFS is a scalable network filesystem. Using common off-the-shelf hardware, you can create large, distributed storage solutions for media streaming, data analysis, and other data- and bandwidth-intensive tasks. GlusterFS is free and open source software.
- [minio](https://www.minio.io/): Minio is a high performance distributed object storage server, designed for 
large-scale private cloud infrastructure. Minio is widely deployed across the world with over 172.6M+ docker pulls.
- [MooseFS](http://www.moosefs.org/): MooseFS is a fault tolerant, network distributed file system. It spreads data over several physical servers which are visible to the user as one resource.
- [FastDFS](https://code.google.com/p/fastdfs/): [FastDFS on Google Code](https://code.google.com/p/fastdfs/), FastDFS is an open source high performance distributed file system. It's major functions include: file storing, file syncing and file accessing, and design for high capacity and load balance.
- [mogilefs](https://github.com/mogilefs/): MogileFS is our open source distributed filesystem.
- [XtreeFS](http://xtreemfs.org/index.php): XtreemFS is a general purpose storage system and covers most storage needs in a single deployment. It is open-source, requires no special hardware or kernel modules, and can be mounted on Linux, Windows and OS X.
- [Taobao File System](http://tfs.taobao.org/): TFS（Taobao !FileSystem）是一个高可扩展、高可用、高性能、面向互联网服务的分布式文件系统，主要针对海量的非结构化数据，它构筑在普通的Linux机器集群上，可为外部提供高可靠和高并发的存储访问。TFS为淘宝提供海量小文件存储，通常文件大小不超过1M，满足了淘宝对小文件存储的需求，被广泛地应用在淘宝各项应用中。它采用了HA架构和平滑扩容，保证了整个文件系统的可用性和扩展性。同时扁平化的数据组织结构，可将文件名映射到文件的物理地址，简化了文件的访问流程，一定程度上为TFS提供了良好的读写性能。
- [seaweedfs](https://github.com/chrislusf/seaweedfs): Seaweed-FS is a simple and highly scalable distributed file system. There are two objectives: to store billions of files! to serve the files fast! Instead of supporting full POSIX file system semantics, Seaweed-FS choose to implement only a key~file mapping. Similar to the word "NoSQL", you can call it as "NoFS".
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
- [TSeer](https://github.com/Tencent/TSeer): TSeer是一套服务注册发现容错的解决方案，是对Tars名字服务功能的轻量化。在腾讯浏览器、应用宝、管家、手机书城、腾讯文学、广点通等众多业务中广泛采用，目前日均承载百亿级别的请求量。

## DNS Server

- [Dnsmasq](http://www.thekelleys.org.uk/dnsmasq/doc.html): Dnsmasq provides network infrastructure for small networks: DNS, DHCP, router advertisement and network boot. It is designed to be lightweight and have a small footprint, suitable for resource constrained routers and firewalls. It has also been widely used for tethering on smartphones and portable hotspots, and to support virtual networking in virtualisation frameworks.
- [PowerDNS](https://www.powerdns.com/): PowerDNS, founded in the late 1990s, is a premier supplier of open source DNS software, services and support. Deployed throughout the world with some of the most demanding users of DNS, we pride ourselves on providing quality software and the very best support available. Since 2015 we are part of Open-Xchange.
- [SkyDNS](https://github.com/skynetservices/skydns): SkyDNS is a distributed service for announcement and discovery of services built on top of etcd. It utilizes DNS queries to discover available services. This is done by leveraging SRV records in DNS, with special meaning given to subdomains, priorities and weights.

## Circuit Breaker

- [Go: Hystrix-go](https://github.com/afex/hystrix-go): Netflix's Hystrix latency and fault tolerance library, for Go
- [Go: gobreaker](https://github.com/sony/gobreaker): Circuit Breaker implemented in Go
  - [Sony gobreaker熔断器源码分析](https://github.com/developer-learning/night-reading-go/blob/master/articles/sony-gobreaker/README.md)
- [Java: Hystrix](https://github.com/Netflix/Hystrix): Hystrix is a latency and fault tolerance library designed to isolate points of access to remote systems, services and 3rd party libraries, stop cascading failure and enable resilience in complex distributed systems where failure is inevitable.
- [C#: Polly](https://github.com/App-vNext/Polly): Polly is a .NET 3.5 / 4.0 / 4.5 / PCL library that allows developers to express transient exception handling policies such as Retry, Retry Forever, Wait and Retry or Circuit Breaker in a fluent manner.
- [C#: Hystrix.NET](https://hystrixnet.codeplex.com): Hystrix.NET is a C# port of Hystrix, which is a latency and fault tolerance library for complex distributed systems.
- [Sentinel](https://github.com/alibaba/Sentinel): A lightweight flow-control library providing high-available protection and monitoring

## Distributed Tracing

- [Open Tracing](http://opentracing.io/): Consistent, expressive, vendor-neutral APIs for distributed tracing and context propagation
- [AppDash](https://github.com/sourcegraph/appdash): Application tracing system for Go, based on Google's Dapper.
- [zipkin](https://github.com/openzipkin/zipkin): Zipkin is a distributed tracing system
- [Jaeger](https://github.com/uber/jaeger): Jaeger, a Distributed Tracing System
  - [Jaeger-client-go](https://github.com/uber/jaeger-client-go): Jaeger Bindings for Go OpenTracing API.

## Cache

- [C: Redis](http://redis.io/): Redis is an open source, BSD licensed, advanced key-value cache and store. It is often referred to as a data structure server since keys can contain strings, hashes, lists, sets, sorted sets, bitmaps and hyperloglogs.
    - [codis](https://github.com/CodisLabs/codis): Proxy based Redis cluster solution supporting pipeline and scaling dynamically
    - [twemproxy](https://github.com/twitter/twemproxy): A fast, light-weight proxy for memcached and redis
    - [redis-cerberus](https://github.com/HunanTV/redis-cerberus): A Redis cluster proxy.
    - [Corvus](https://github.com/eleme/corvus): A fast and lightweight Redis Cluster Proxy for Redis 3.0
    - [CacheCloud](https://github.com/sohutv/cachecloud):  CacheCloud提供一个Redis云管理平台：实现多种类型(Redis Standalone、Redis Sentinel、Redis Cluster)自动部署、解决Redis实例碎片化现象、提供完善统计、监控、运维功能、减少运维成本和误操作，提高机器的利用率，提供灵活的伸缩性，提供方便的接入客户端。
- [Pika](https://github.com/Qihoo360/pika): Pika is a nosql compatible with redis, it is developed by Qihoo's DBA and infrastructure team
- [C: Memcached](http://memcached.org/): Free & open source, high-performance, distributed memory object caching system, generic in nature, but intended for use in speeding up dynamic web applications by alleviating database load. Memcached is an in-memory key-value store for small chunks of arbitrary data (strings, objects) from results of database calls, API calls, or page rendering. Memcached is simple yet powerful. Its simple design promotes quick deployment, ease of development, and solves many problems facing large data caches. Its API is available for most popular languages.
- [Go: Groupcahe](https://github.com/golang/groupcache): groupcache is a caching and cache-filling library, intended as a replacement for memcached in many cases.
- [Java: Hazelcast](https://github.com/hazelcast/hazelcast): Hazelcast is a clustering and highly scalable data distribution platform.
- [Java: Infinispan](http://infinispan.org): Infinispan is a distributed in-memory key/value data store with optional schema, available under the Apache License 2.0. It can be used both as an embedded Java library and as a language-independent service accessed remotely over a variety of protocols (HotRod, REST, Memcached and WebSockets). It offers advanced functionality such as transactions, events, querying and distributed processing.


## Database Driver

- [ShardingSphere](https://shardingsphere.apache.org/): Apache ShardingSphere is an open-source ecosystem consisted of a set of distributed database middleware solutions, including 3 independent products, Sharding-JDBC, Sharding-Proxy & Sharding-Sidecar (Planning). They all provide functions of data sharding, distributed transaction and database orchestration, applicable in a variety of situations such as Java isomorphism, heterogeneous language and cloud native.

## Other

- [Golang: Sonyflake](https://github.com/sony/sonyflake): A distributed unique ID generator inspired by Twitter's Snowflake
