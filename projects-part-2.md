# Projects about Distributed Architecture

## Data Exchange Format

- [Portocol Buffer](https://developers.google.com/protocol-buffers/): Protocol buffers are Google's language-neutral, platform-neutral, extensible mechanism for serializing structured data – think XML, but smaller, faster, and simpler.
- [Message Pack](http://msgpack.org/): MessagePack is an efficient binary serialization format. It lets you exchange data among multiple languages like JSON. But it's faster and smaller. Small integers are encoded into a single byte, and typical short strings require only one extra byte in addition to the strings themselves.
- [Apache Thrift](http://thrift.apache.org/): Thrift源于大名鼎鼎的facebook之手，在2007年facebook提交Apache基金会将Thrift作为一个开源项目，对于当时的facebook来说创造thrift是为了解决facebook系统中各系统间大数据量的传输通信以及系统之间语言环境不同需要跨平台的特性。所以thrift可以支持多种程序语言，例如: C++, C#, Cocoa, Erlang Haskell, Java, Ocami, Perl, PHP, Python, Ruby, Smalltalk. 在多种不同的语言之间通信thrift可以作为二进制的高性能的通讯中间件，支持数据(对象)序列化和多种类型的RPC服务。Thrift适用于程序对程序静态的数据交换，需要先确定好他的数据结构，他是完全静态化的，当数据结构发生变化时，必须重新编辑IDL文件，代码生成，再编译载入的流程，跟其他IDL工具相比较可以视为是Thrift的弱项，Thrift适用于搭建大型数据交换及存储的通用工具，对于大型系统中的内部数据传输相对于JSON和xml无论在性能、传输大小上有明显的优势。
- [Apache Avro](http://avro.apache.org/): Apache Avro™ is a data serialization system.
- [Cap’n Proto](https://capnproto.org/index.html): Cap’n Proto is an insanely fast data interchange format and capability-based RPC system. Think JSON, except binary. Or think Protocol Buffers, except faster. In fact, in benchmarks, Cap’n Proto is INFINITY TIMES faster than Protocol Buffers.
- [Microsoft bond](https://github.com/Microsoft/bond): Bond is a cross-platform framework for working with schematized data. It supports cross-language de/serialization and powerful generic mechanisms for efficiently manipulating data. Bond is broadly used at Microsoft in high scale services.
- [JSON](http://json.org/): JSON (JavaScript Object Notation) is a lightweight data-interchange format. It is easy for humans to read and write. It is easy for machines to parse and generate. It is based on a subset of the JavaScript Programming Language, Standard ECMA-262 3rd Edition - December 1999. JSON is a text format that is completely language independent but uses conventions that are familiar to programmers of the C-family of languages, including C, C++, C#, Java, JavaScript, Perl, Python, and many others. These properties make JSON an ideal data-interchange language.
    - [JSON Schema](http://json-schema.org/)
    - [JSON Schema Generator](http://jsonschema.net/)

## Distributed Application Framework

- [akka.net](http://getakka.net/): a toolkit and runtime for building highly concurrent, distributed, and fault tolerant event-driven applications on .NET & Mono.
- [akka](http://akka.io/): Akka is a toolkit and runtime for building highly concurrent, distributed, and resilient message-driven applications on the JVM. The power of Akka is also available on the .NET Framework and Mono via the Akka.NET project.
- [Zyan Communication Framework](http://zyan.com.de/): Easy to use distributed application framework for .NET, Mono and Xamarin.Android.
- [Vert.x](http://vertx.io): Vert.x is a tool-kit for building reactive applications on the JVM.

## Service Bus

- [MassTransit](http://masstransit-project.com/): Lean Service Bus for .NET
- [Rebus](https://github.com/rebus-org/Rebus): Rebus is a lean service bus implementation for .NET, similar in nature to NServiceBus and MassTransit, only leaner
- [NServiceBus](https://github.com/Particular): The most popular service bus for .NET
- [Shuttle-ESB](http://shuttle.github.io/shuttle-esb/): A highly configurable free open-source enterprise service bus that provides you with a mechanism to create Autonomous Business Components that are loosely coupled. This enables you to develop and deploy specific business functionality that can be independently versioned.
- [Rhino ESB](https://github.com/hibernating-rhinos/rhino-esb): Rhino Service Bus is a messaging framework that supports transactional, durable, reliable, distributed, asynchronous messaging. Rhino Service Bus currently supports two transports MSMQ and Rhino.Queues.

## Messsage Queue

- [RabbitMQ](http://www.rabbitmq.com/): RabbitMQ is a messaging broker - an intermediary for messaging. It gives your applications a common platform to send and receive messages, and your messages a safe place to live until received.
    - [RabbitMQ Internals](https://github.com/rabbitmq/internals): This project aims to explain how RabbitMQ works internally. The goal is to make it easier to contribute for newcomers to the project, and at the same time have a common repository of knowledge to be shared across the project contributors.
- [ZeroMQ](http://zeromq.org/): ZeroMQ (also known as ØMQ, 0MQ, or zmq) looks like an embeddable networking library but acts like a concurrency framework. It gives you sockets that carry atomic messages across various transports like in-process, inter-process, TCP, and multicast. You can connect sockets N-to-N with patterns like fan-out, pub-sub, task distribution, and request-reply. It's fast enough to be the fabric for clustered products. Its asynchronous I/O model gives you scalable multicore applications, built as asynchronous message-processing tasks. It has a score of language APIs and runs on most operating systems.
- [NetMQ](https://github.com/zeromq/netmq): NetMQ is 100% native C# port of ZeroMQ
- [beanstalkd](http://kr.github.io/beanstalkd/): Beanstalk is a simple, fast work queue. Its interface is generic, but was originally designed for reducing the latency of page views in high-volume web applications by running time-consuming tasks asynchronously.
- [Apache ActiveMQ](http://activemq.apache.org/): Apache ActiveMQ ™ is the most popular and powerful open source messaging and Integration Patterns server. Apache ActiveMQ is fast, supports many Cross Language Clients and Protocols, comes with easy to use Enterprise Integration Patterns and many advanced features while fully supporting JMS 1.1 and J2EE 1.4. Apache ActiveMQ is released under the Apache 2.0 License.
- [NSQ](https://github.com/bitly/nsq): NSQ is a realtime distributed messaging platform designed to operate at scale, handling billions of messages per day.

## Load Balance

- [LVS](http://www.linuxvirtualserver.org/): The Linux Virtual Server is a highly scalable and highly available server built on a cluster of real servers, with the load balancer running on the Linux operating system. The architecture of the server cluster is fully transparent to end users, and the users interact as if it were a single high-performance virtual server.
- [HAProxy](http://www.haproxy.org/): HAProxy is a free, very fast and reliable solution offering high availability, load balancing, and proxying for TCP and HTTP-based applications.
    - [Bamboo](https://github.com/QubitProducts/bamboo): HAProxy auto configuration and auto service discovery for Mesos Marathon
- [Nginx](http://wiki.nginx.org/Main): Nginx (pronounced engine-x) is a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
- [Pen](http://siag.nu/pen/): Pen is a load balancer for "simple" TCP-based protocols such as HTTP or SMTP. It allows several servers to appear as one to the outside. It automatically detects servers that are down and distributes clients among the available servers. This gives high availability and scalable performance.
- [Balance](http://www.inlab.de/balance.html): Balance is a simple but powerful generic TCP proxy with round-robin load balancing and failover mechanisms. Its behavior can be controlled at runtime using a simple command line syntax. Balance supports IPv6 on the listening side, which makes it a very useful tool for IPv6 migration of IPv4 only services and servers.
- [keepalived](http://www.keepalived.org/): Keepalived is a routing software written in C. The main goal of this project is to provide simple and robust facilities for loadbalancing and high-availability to Linux system and Linux based infrastructures.

## Reverse Proxy

- [Nginx](http://wiki.nginx.org/Main): Nginx (pronounced engine-x) is a free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server.
- [Varnish](https://www.varnish-cache.org/): Varnish是一款高性能且开源的反向代理服务器和http加速器。与传统的Squid相比，Varnish具有性能更高、速度更快、管理更方便 等诸多优点。作者Poul-Henning Kamp是FreeBSD的内核开发者之一。Varnish采用全新的软件体系架构，和现在的硬件提交配合紧密。在1975年时，储存媒介只有两种：内存 与硬盘。但现在计算 机系统的内存除了主存外，还包括了cpu内的L1、L2，甚至有L3快取。硬盘上也有自己的快取装置，因此squid cache自行处理物件替换的架构不可能得知这些情况而做到最佳化，但操作系统可以得知这些情况，所以这部份的工作应该交给操作系统处理，这就是 Varnish cache设计架构。挪威最大的在线报纸Verdens Gang使用3台Varnish代替了原来的12台squid，性能居然比以前更好，这是Varnish最成功的应用案例。
- [Squid](http://www.squid-cache.org/): Squid is a caching proxy for the Web supporting HTTP, HTTPS, FTP, and more. It reduces bandwidth and improves response times by caching and reusing frequently-requested web pages. Squid has extensive access controls and makes a great server accelerator. It runs on most available operating systems, including Windows and is licensed under the GNU GPL.

## Distributed File System

- [Ceph](http://ceph.com/): Ceph is a distributed object store and file system designed to provide excellent performance, reliability and scalability. See more at: http://ceph.com/#sthash.46aGKE2z.dpuf
- [MooseFS](http://www.moosefs.org/): MooseFS is a fault tolerant, network distributed file system. It spreads data over several physical servers which are visible to the user as one resource.
- [Glusterfs](http://www.gluster.org/): GlusterFS is a scalable network filesystem. Using common off-the-shelf hardware, you can create large, distributed storage solutions for media streaming, data analysis, and other data- and bandwidth-intensive tasks. GlusterFS is free and open source software.
- [FastDFS](https://code.google.com/p/fastdfs/): [FastDFS on Google Code](https://code.google.com/p/fastdfs/), FastDFS is an open source high performance distributed file system. It's major functions include: file storing, file syncing and file accessing, and design for high capacity and load balance.
- [mogilefs](https://github.com/mogilefs/): MogileFS is our open source distributed filesystem.
- [XtreeFS](http://xtreemfs.org/index.php): XtreemFS is a general purpose storage system and covers most storage needs in a single deployment. It is open-source, requires no special hardware or kernel modules, and can be mounted on Linux, Windows and OS X.
- [Taobao File System](http://tfs.taobao.org/): TFS（Taobao !FileSystem）是一个高可扩展、高可用、高性能、面向互联网服务的分布式文件系统，主要针对海量的非结构化数据，它构筑在普通的Linux机器集群上，可为外部提供高可靠和高并发的存储访问。TFS为淘宝提供海量小文件存储，通常文件大小不超过1M，满足了淘宝对小文件存储的需求，被广泛地应用在淘宝各项应用中。它采用了HA架构和平滑扩容，保证了整个文件系统的可用性和扩展性。同时扁平化的数据组织结构，可将文件名映射到文件的物理地址，简化了文件的访问流程，一定程度上为TFS提供了良好的读写性能。
- [seaweedfs](https://github.com/chrislusf/seaweedfs): Seaweed-FS is a simple and highly scalable distributed file system. There are two objectives: to store billions of files! to serve the files fast! Instead of supporting full POSIX file system semantics, Seaweed-FS choose to implement only a key~file mapping. Similar to the word "NoSQL", you can call it as "NoFS".
- [GlusterFS](http://www.gluster.org/): GlusterFS is a scalable network filesystem. Using common off-the-shelf hardware, you can create large, distributed storage solutions for media streaming, data analysis, and other data- and bandwidth-intensive tasks. GlusterFS is free and open source software.

## Configuration Management

- [Confd](https://github.com/kelseyhightower/confd): Manage local application configuration files using templates and data from etcd or consul
- [Consul Template](https://github.com/hashicorp/consul-template): This project provides a convenient way to populate values from Consul into the filesystem using the consul-template daemon.
- [disconf](https://github.com/knightliao/disconf): Distributed Configuration Management Platform(分布式配置管理平台)
- [Qconf](https://github.com/Qihoo360/QConf): Qihoo Distrubuted Configuration Management System
- [super diamond](https://github.com/melin/super-diamond): 配置管理系统
- [XDiamond](https://github.com/hengyunabc/xdiamond): 全局配置中心，存储应用的配置项，解决配置混乱分散的问题。名字来源于淘宝的开源项目diamond，前面加上一个字母X以示区别。
- [archaius](https://github.com/Netflix/archaius): Library for configuration management API

## 分布式协调(Service Discovery, Name Service)

- [Apache Zookeeper](http://zookeeper.apache.org/): ZooKeeper is a centralized service for maintaining configuration information, naming, providing distributed synchronization, and providing group services. All of these kinds of services are used in some form or another by distributed applications. Each time they are implemented there is a lot of work that goes into fixing the bugs and race conditions that are inevitable. Because of the difficulty of implementing these kinds of services, applications initially usually skimp on them ,which make them brittle in the presence of change and difficult to manage. Even when done correctly, different implementations of these services lead to management complexity when the applications are deployed.
- [etcd](https://github.com/coreos/etcd): A distributed consistent key-value store for shared configuration and service discovery
- [SkyDNS](https://github.com/skynetservices/skydns): SkyDNS is a distributed service for announcement and discovery of services built on top of etcd. It utilizes DNS queries to discover available services. This is done by leveraging SRV records in DNS, with special meaning given to subdomains, priorities and weights.
- [consul](https://www.consul.io/): Consul 简化了分布式环境中的服务的注册和发现流程，通过 HTTP 或者 DNS 接口发现。支持外部 SaaS 提供者等。

## 熔断器

- [Polly](https://github.com/App-vNext/Polly): Polly is a .NET 3.5 / 4.0 / 4.5 / PCL library that allows developers to express transient exception handling policies such as Retry, Retry Forever, Wait and Retry or Circuit Breaker in a fluent manner.
- [Hystrix](https://github.com/Netflix/Hystrix): Hystrix is a latency and fault tolerance library designed to isolate points of access to remote systems, services and 3rd party libraries, stop cascading failure and enable resilience in complex distributed systems where failure is inevitable.
- [Hystrix.NET](https://hystrixnet.codeplex.com): Hystrix.NET is a C# port of Hystrix, which is a latency and fault tolerance library for complex distributed systems.
