<!-- TOC -->

- [Project about DevOps](#project-about-devops)
  - [Code Repository](#code-repository)
  - [Code Analysis and Metrics](#code-analysis-and-metrics)
  - [Scaffolding](#scaffolding)
  - [Build](#build)
  - [Continuous Integration](#continuous-integration)
  - [Artifact Repository](#artifact-repository)
  - [Automation](#automation)
  - [Unit Testing](#unit-testing)
  - [Database Testing](#database-testing)
  - [Database Management](#database-management)
  - [Automated Acceptance Testing/BDD](#automated-acceptance-testingbdd)
  - [API Testing](#api-testing)
  - [Performance Testing](#performance-testing)
  - [System Monitor](#system-monitor)
  - [Gather System Information](#gather-system-information)
  - [Process Supervisor](#process-supervisor)
  - [User Behavior Collection & Analysis](#user-behavior-collection--analysis)
  - [Infrastructure Management](#infrastructure-management)
  - [OS Configuration Management](#os-configuration-management)
  - [Terminal](#terminal)
  - [Container](#container)
  - [Virtualization](#virtualization)
  - [Serverless](#serverless)
  - [Misc](#misc)

<!-- /TOC -->


# Project about DevOps

## Code Repository

- [C: Git](http://www.git-scm.com/): Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
	- [Golang: git-appraise](https://github.com/google/git-appraise): Distributed Code Review For Git
	- [Golang: git-lfs](https://git-lfs.github.com/): An open source Git extension for versioning large files
	- [Java: gerrit](https://www.gerritcodereview.com/): Gerrit provides web based code review and repository management for the Git version control system.
	- [Golang: Gogs](http://gogs.io/): 极易搭建的自助 Git 服务
	- [Golang: Gitea](https://github.com/go-gitea/gitea)
	- [Ruby: Gitlab](https://about.gitlab.com/): Open source git server
	- [Perl: gitolite](https://github.com/sitaramc/gitolite): Hosting git repositories -- Gitolite allows you to setup git hosting on a central server, with very fine-grained access control and many (many!) more powerful features.
	- [C#: bonobo git server](https://bonobogitserver.com/): Simple git server for Windows. Set up your own self hosted git server on IIS for Windows. Manage users and have full control over your repositories with a nice user friendly graphical interface.

## Code Analysis and Metrics

- [Golang: Go Meta Linter](https://github.com/alecthomas/gometalinter): Concurrently run Go lint tools and normalise their output
- [JavaScript: ESlint](http://eslint.org/): The pluggable linting utility for JavaScript and JSX
    - [JSCS — JavaScript Code Style](http://jscs.info/): **JSCS has merged with ESLint!** JSCS is a code style linter and formatter for your style guide
- [SonarQube](http://www.sonarqube.org/): SonarQube is an open platform to manage code quality.
- [.NET: StyleCop](https://stylecop.codeplex.com/) - StyleCop analyzes C# source code to enforce a set of style and consistency rules
- [.NET: OpenCover](https://github.com/OpenCover/opencover): A code coverage tool for .NET 2 and above, support for 32 and 64 processes with both branch and sequence points; roots proudly based in PartCover

## Scaffolding

- [Node: Yeoman](http://yeoman.io): The Yeoman workflow is comprised of three core tools for improving your productivity and satisfaction when building a web app.

## Build

- [Make](https://www.gnu.org/software/make/manual/make.html): GNU Make手册
- [CMake](https://cmake.org/): CMake is an open-source, cross-platform family of tools designed to build, test and package software. CMake is used to control the software compilation process using simple platform and compiler independent configuration files, and generate native makefiles and workspaces that can be used in the compiler environment of your choice. The suite of CMake tools were created by Kitware in response to the need for a powerful, cross-platform build environment for open-source projects such as ITK and VTK.
- [Bazel](http://bazel.io/): Bazel is Google's own build tool, now publicly available in Beta. Bazel has built-in support for building both client and server software, including client applications for both Android and iOS platforms. It also provides an extensible framework that you can use to develop your own build rules. Bazel is a build tool which coordinates builds and run tests. It works with source files written in any language, with native support for Java, C, C++ and Python. Bazel produces builds and runs tests for multiple platforms.
- [Facebook Buck](https://buckbuild.com/): Buck is a build system developed and used by Facebook. It encourages the creation of small, reusable modules consisting of code and resources, and supports a variety of languages on many platforms.
- [Java: Gradle](http://gradle.org/): OPEN SOURCE BUILD AUTOMATION. Get started with: Java / JVM | Android | Native (C / C++) | Web and many more!
	- [Java: Maven](http://maven.apache.org/): Apache Maven is a software project management and comprehension tool. Based on the concept of a project object model (POM), Maven can manage a project's build, reporting and documentation from a central piece of information.
- [MSBuild](https://github.com/Microsoft/msbuild) - The Microsoft Build Engine (MSBuild) is the build platform for .NET and Visual Studio
	- [Psake](https://github.com/psake/psake) - .NET-based build automation tool written in PowerShell
	- [Invoke-Build](https://github.com/nightroman/Invoke-Build) - PowerShell build and test automation tool inspired by Psake.
- [Wixtoolset](http://wixtoolset.org/): The WiX toolset builds Windows installation packages from XML source code. The toolset integrates seamlessly into build processes.

参考：

- [Make命令教程](http://www.ruanyifeng.com/blog/2015/02/make.html)

## Continuous Integration

- [Jenkins-CI](http://jenkins-ci.org/): An extensible open source continuous integration server
  - [janky](https://github.com/github/janky): Continuous integration server built on top of Jenkins and Hubot
- [Fabric8](https://fabric8.io/): fabric8 is an end to end development platform spanning ideation to production for the creation of cloud native applications and microservices. You can build, test and deploy your applications via Continuous Delivery pipelines then run and manage them with Continuous Improvement and ChatOps
- [Concourse CI](https://github.com/concourse/concourse): CI that scales with your project.
- [Walle](https://github.com/meolu/walle-web): walle - 瓦力 Devops开源项目代码部署平台
- [drone](https://github.com/drone/drone): Drone is a Continuous Delivery system built on container technology. Drone uses a simple yaml configuration file, a superset of docker-compose, to define and execute Pipelines inside Docker containers.
- [spinnaker](http://www.spinnaker.io/): Spinnaker is an open source, multi-cloud continuous delivery platform for releasing software changes with high velocity and confidence.
- [CruiseControl.NET](http://www.cruisecontrolnet.org/) - an Automated Continuous Integration server, implemented using the .NET Framework
- [Go.cd](http://www.go.cd/): Automate and streamline the build-test-release cycle for worry-free, continuous delivery of your product.
- [Buildbot](http://buildbot.net/index.html): Python-based continuous integration testing framework; your pull requests are more than welcome!
- [MyGet](http://www.myget.org/) - Continuous Integration and Deployment, Hosted Package Repository for NuGet, NPM, Bower and VSIX. [Free for OSS] [$]


## Artifact Repository

- [Nexus Repository OSS](https://www.sonatype.com/nexus-repository-oss): The free artifact repository with universal support for popular formats. 

参考：

- [mvn repository](https://mvnrepository.com/)


## Automation

- [Python: Twill](http://twill.idyll.org/): a simple scripting language for Web browsing
- [Python: Mechanize](https://github.com/python-mechanize/mechanize): Automate interaction with HTTP web servers
- [Hubot](https://hubot.github.com/): GitHub, Inc., wrote the first version of Hubot to automate our company chat room. Hubot knew how to deploy the site, automate a lot of tasks, and be a source of fun in the company. Eventually he grew to become a formidable force in GitHub. But he led a private, messy life. So we rewrote him.


## Unit Testing

- [Golang: Testify](https://github.com/stretchr/testify): A sacred extension to the standard go testing package
- [Golang: Go frisby](https://github.com/verdverm/frisby): API testing framework inspired by frisby-js
- [Golang: httpexpect](https://github.com/gavv/httpexpect): End-to-end HTTP and REST API testing for Go.
- [Golang: govcr](https://github.com/seborama/govcr): Record and replay HTTP interactions for offline unit / behavioural / integration tests thereby acting as an HTTP mock.
- [.NET: NUnit](https://github.com/nunit/nunit-framework)
- [.NET: xUnit](https://github.com/xunit/xunit) - xUnit.net is a free, open source, community-focused unit testing tool for the .NET Framework
- [.NET: Fluent Assertions](https://github.com/fluentassertions/fluentassertions): Fluent Assertions is a set of .NET extension methods that allow you to more naturally specify the expected outcome of a TDD or BDD-style test.
- [.NET: AutoFixture](https://github.com/AutoFixture/AutoFixture) - AutoFixture is an open source framework for .NET designed to minimize the 'Arrange' phase of your unit tests
- [.NET: Moq](https://github.com/Moq/moq4) - The most popular and friendly mocking framework for .NET
- [.NET: Rhino Mocks](https://github.com/ayende/rhino-mocks) - Dynamic Mocking Framework for .NET
- [.NET: NSubstitute](http://nsubstitute.github.io/) - A friendly substitute for .NET mocking frameworks
- [.NET: Shouldly](https://github.com/shouldly/shouldly): Should testing for .net - the way Asserting *Should* be!

## Database Testing

- [dbUnit](http://dbunit.sourceforge.net/intro.html): database unit testing
- [TSQLT](http://tsqlt.org/): tSQLt is a database unit testing framework for Microsoft SQL Server. tSQLt is compatible with SQL Server 2005 (service pack 2 required) and above on all editions.
- [DbFit](http://dbfit.github.io/dbfit/index.html): Test-driven database development. Write readable, easy-to-maintain unit and integration tests for your database code.

## Database Management

- [SqlPad](http://rickbergfalk.github.io/sqlpad/): Run SQL in your browser...Supports Postgres, MySQL, SQL Server and Vertica.
- [Perl: sqitch](http://sqitch.org/): Sqitch is a database change management application. It currently supports PostgreSQL 8.4+, SQLite 3.7.11+, MySQL 5.0+, Oracle 10g+, Firebird 2.0+, and Vertica 6.0+.
- [Golang: goose](https://bitbucket.org/liamstask/goose): goose is a database migration tool. You can manage your database's evolution by creating incremental SQL or Go scripts.

## Automated Acceptance Testing/BDD

- [Selenium](http://www.seleniumhq.org/): Selenium is a suite of tools to automate web browsers across many platforms.
- [Java: Cucumber](https://cucumber.io/): Cucumber is a software tool that computer programmers use for testing other software. It runs automated acceptance tests written in a behavior-driven development (BDD) style.
	- [cucumber.js](https://github.com/cucumber/cucumber-js): Cucumber, the popular Behaviour-Driven Development tool, brought to your JavaScript stack.It runs on both Node.js and modern web browsers.
	- [SpecFlow](http://www.specflow.org/): Cucumber for .NET. The open source solution trusted by .NET devs around the world.
- [Java: JBehave](http://jbehave.org): JBehave is a framework for Behaviour-Driven Development (BDD). BDD is an evolution of test-driven development (TDD) and acceptance-test driven design, and is intended to make these practices more accessible and intuitive to newcomers and experts alike. It shifts the vocabulary from being test-based to behaviour-based, and positions itself as a design philosophy.
- [JavaScript: Jasmine](https://github.com/jasmine/jasmine): Jasmine is a Behavior Driven Development testing framework for JavaScript. It does not rely on browsers, DOM, or any JavaScript framework. Thus it's suited for websites, Node.js projects, or anywhere that JavaScript can run.
- [Go: Gauge](https://gauge.org/): Test Automation you'll actually like Simple. Collaborative. Adaptable.
- [Go: ginkgo](https://github.com/onsi/ginkgo): BDD Testing Framework for Go
- [Go: goconvey](https://github.com/smartystreets/goconvey): Go testing in the browser. Integrates with `go test`. Write behavioral tests in Go. 
- [Go: go-fuzz](https://github.com/dvyukov/go-fuzz): Randomized testing for Go
- [Python:ROBOT FRAMEWORK](https://robotframework.org/#introduction): Robot Framework is a generic open source automation framework for acceptance testing, acceptance test driven development (ATDD), and robotic process automation (RPA).

## API Testing

- [Postman](https://www.getpostman.com/)
- [yapi](https://github.com/YMFE/yapi)

## Performance Testing

- [Python: Lucust](http://locust.io/): Define user behaviour with Python code, and swarm your system with millions of simultaneous users.
- [Web Bench](http://home.tiscali.cz:8080/~cz210552/webbench.html): Web Bench是一个简单的web或者web代理服务的基准测试工具。（它）使用fork()模拟多个客户端并且可以发起HTTP/0/9-HTTP/1.1的请求。这个基准测试不是非常符合实际情况，但是可以测试出你的HTTP服务是否可以处理多个客户同时访问而不会把你的机器弄挂掉。这个工具可以获得服务的两个指标：每分钟响应请求数量（pages/min）和每秒钟传输数据量（bytes/sec）。
- [Siege](https://www.joedog.org/siege-home/): Siege（英文意思是围攻）是一个压力测试和评测工具，设计用于WEB开发这评估应用在压力下的承受能力：可以根据配置对一个WEB站点进行多用户的并发访问，记录每个用户所有请求过程的相应时间，并在一定数量的并发访问下重复进行。 Siege 支持基本的认证，cookies， HTTP 和 HTTPS 协议。
- [AB - Apache HTTP server benchmarking tool](http://jmeter.apache.org/): ab命令会创建很多的并发访问线程，模拟多个访问者同时对某一URL地址进行访问。它的测试目标是基于URL的，因此，既可以用来测试Apache的负载压力，也可以测试nginx、lighthttp、tomcat、IIS等其它Web服务器的压力。ab命令对发出负载的计算机要求很低，既不会占用很高CPU，也不会占用很多内存，但却会给目标服务器造成巨大的负载，其原理类似CC攻击。
- [Java: Apache JMeter](http://jmeter.apache.org/): Apache JMeter是一个专门为运行和服务器装载测试而设计的、100％的纯Java桌面运行程序。原先它是为Web/HTTP测试而设计的，但是它已经扩展以支持各种各样的测试模块。它和用于HTTP和SQL数据库（使用JDBC）的模块一起运送。它可以用来测试静止资料库或者活动资料库中的服务器的运行情况，可以用来模拟对服务器或者网络系统加以重负荷以测试它的抵抗力，或者用来分析不同负荷类型下的所有运行情况。它也提供了一个可替换的界面用来定制数据显示，测试同步及测试的创建和执行。
    - [Badboy](http://www.badboy.com.au/): Badboy is a powerful tool designed to aid in testing and development of complex dynamic applications. Badboy makes web testing and development easier with dozens of features including a simple yet comprehensive capture/replay interface, powerful load testing support, detailed reports, graphs and much more!
    - [Ruby: ruby-jmeter](https://github.com/flood-io/ruby-jmeter): A Ruby based DSL for building JMeter test plans
- [Scala: Gatling](http://gatling.io/): Gatling is an open-source load testing framework based on Scala, Akka and Netty
- [Erlang: Tsung](http://tsung.erlang-projects.org/): Tsung is an open-source multi-protocol distributed load testing tool. It can be used to stress HTTP, WebDAV, SOAP, PostgreSQL, MySQL, LDAP, MQTT and Jabber/XMPP servers. Tsung is a free software released under the GPLv2 license.
- [.NET: West Wind Websurge](http://websurge.west-wind.com/): We believe that testing HTTP requests and load testing a site should be easy - something that takes a few minutes to set up and then runs on a regular basis during the development process, so that you can monitor performance of your site while you are building it. To this end we built West Wind WebSurge with the developer and testers in mind to make it easy to create HTTP requests or entire sessions, and then easily play back either individual URLs for development response testing, or for full-on testing under heavy load. Sessions are stored in plain text files so that they can be easily stored with projects or shared via source control for all users to have access.
- [C: wrk](https://github.com/wg/wrk): 
wrk is a modern HTTP benchmarking tool capable of generating significant load when run on a single multi-core CPU. It combines a multithreaded design with scalable event notification systems such as epoll and kqueue.
    - [go-wrk](https://github.com/tsliwowicz/go-wrk): go-wrk - a HTTP benchmarking tool based in spirit on the excellent wrk tool
- [C: Tcpkali](https://github.com/machinezone/tcpkali): Fast multi-core TCP and WebSockets load generator.
- [C: TCPCopy](https://github.com/session-replay-tools/tcpcopy): TCPCopy is a TCP stream replay tool to support real testing of Internet server applications.
- [Go: Gor](https://github.com/buger/gor): Gor is a simple http traffic replication tool written in Go. Its main goal is to replay traffic from production servers to staging and dev environments.
- [Go: Goreplay](https://github.com/buger/goreplay): GoReplay is an open-source tool for capturing and replaying live HTTP traffic into a test environment in order to continuously test your system with real data.
- [Go: Toxy](https://github.com/h2non/toxy): Hackable HTTP proxy to simulate server failure scenarios and unexpected network conditions


## System Monitor

- [Go: Prometheus](http://prometheus.io/): An open-source service monitoring system and time series database.
    - [Thanos](https://github.com/improbable-eng/thanos): Highly available Prometheus setup with long term storage capabilities.
    - [Grafana](http://grafana.org/): Grafana is a leading open source application for visualizing large-scale measurement data.
- [Alerta monitoring system](http://docs.alerta.io/en/latest/index.html): The alerta monitoring system is a tool used to consolidate and de-duplicate alerts from multiple sources for quick ‘at-a-glance’ visualisation. With just one system you can monitor alerts from many other monitoring tools on a single screen.
- [Graphite - Scalable Realtime Graphing](http://graphite.wikidot.com/): Graphite 是一个用于采集网站实时信息并进行统计的开源项目，可用于采集多种网站服务运行状态信息。Graphite服务平均每分钟有4800次更新操作。实践已经证实要监测网站发发生什么是非常有用的，它的简单文本协议和绘图功能可以方便地即插即 用的方式用于任何需要监控的系统上
- [Nagios](https://www.nagios.org/): Nagios Is The Industry Standard In IT Infrastructure Monitoring. Achieve instant awareness of IT infrastructure problems, so downtime doesn't adversely affect your business.
- [Icinga](https://www.icinga.org/): ICINGA项目是 由Michael Luebben、HendrikB?cker和JoergLinge等人发起的，他们都是现有的Nagios项目社区委员会的成员，他们承诺，新的开源项 目将完全兼容以前的Nagios应用程序及扩展功能。在新项目的网站上，他们是如此定义ICINGA的，这将是一个介于Nagios社区版和企业版间的产 品。特别将致力于解决Nagios项目现在的问题，比如不能及时处理Nagios项目的bug、新功能不能及时添加等。还有在新的ICINGA项目中，将 更好的实现数据库集成方面的功能，标准化第三发应用程序的接口等。
- [Zabbix](http://www.zabbix.com/): Zabbix is the ultimate enterprise-level software designed for real-time monitoring of millions of metrics collected from tens of thousands of servers, virtual machines and network devices.
- [Riemann](http://riemann.io/): Riemann aggregates events from your servers and applications with a powerful stream processing language. Send an email for every exception in your app. Track the latency distribution of your web app. See the top processes on any host, by memory and CPU. Combine statistics from every Riak node in your cluster and forward to Graphite. Track user activity from second to second.
- [Ganglia Monitoring System](http://ganglia.info/): Ganglia is a scalable distributed monitoring system for high-performance computing systems such as clusters and Grids. It is based on a hierarchical design targeted at federations of clusters. It leverages widely used technologies such as XML for data representation, XDR for compact, portable data transport, and RRDtool for data storage and visualization. It uses carefully engineered data structures and algorithms to achieve very low per-node overheads and high concurrency. The implementation is robust, has been ported to an extensive set of operating systems and processor architectures, and is currently in use on thousands of clusters around the world. It has been used to link clusters across university campuses and around the world and can scale to handle clusters with 2000 nodes.
- [Python: Sentry](https://github.com/getsentry): Real-time crash reporting for your web apps, mobile apps, and games.
- [Go: bosun](https://github.com/bosun-monitor/bosun): Bosun is an open-source, MIT licensed, monitoring and alerting system by Stack Exchange. It has an expressive domain specific language for evaluating alerts and creating detailed notifications. It also lets you test your alerts against history for a faster development experience.
- [Open-Falcon企业级监控系统解决方案](http://open-falcon.com/): Open-Falcon 是小米运维部开源的一款互联网企业级监控系统解决方案.
- [Opserver](https://github.com/opserver/opserver): Opserver is a monitoring system by the team at Stack Exchange, home of Stack Overflow.

## Gather System Information

- [Tsar](https://github.com/kongjian/tsar): Tsar (Taobao System Activity Reporter) is a monitoring tool, which can be used to gather and summarize system information, e.g. CPU, load, IO, and application information, e.g. nginx, HAProxy, Squid, etc. The results can be stored at local disk or sent to Nagios.
- [collectd](http://collectd.org/): collectd is a daemon which collects system performance statistics periodically and provides mechanisms to store the values in a variety of ways, for example in RRD files.
- [osquery](https://github.com/facebook/osquery): SQL powered operating system instrumentation, monitoring, and analytics.
- [cAdvisor](https://github.com/google/cadvisor): Analyzes resource usage and performance characteristics of running containers.

## Process Supervisor

- [Supervisor](http://supervisord.org): Supervisor is a client/server system that allows its users to control a number of processes on UNIX-like operating systems.
- [PM2](https://github.com/Unitech/pm2): Production process manager for Node.js applications with a built-in load balancer https://app.keymetrics.io/


## User Behavior Collection & Analysis

- [PHP: Piwik](http://piwik.org/): Piwik is an open analytics platform currently used by individuals, companies and governments all over the world. With Piwik, your data will always be yours. Learn why Piwik is the right web analytics tool for you below.
- [Open Web Analytics](http://www.openwebanalytics.com/): Open Web Analytics (OWA) is open source web analytics software that you can use to track and analyze how people use your websites and applications. OWA is licensed under GPL and provides website owners and developers with easy ways to add web analytics to their sites using simple Javascript, PHP, or REST based APIs.
- [Snowplow - the event analytics platform](http://snowplowanalytics.com/): Have every single event, from your websites, mobile apps, desktop applications and server-side systems, stored in your own data warehouse and available to action in real-time.
- [tracking.js](http://trackingjs.com/): The tracking.js library brings different computer vision algorithms and techniques into the browser environment. By using modern HTML5 specifications, we enable you to do real-time color tracking, face detection and much more — all that with a lightweight core (~7 KB) and intuitive interface.


## Infrastructure Management

- [C++: Apache Mesos](http://mesos.apache.org/): Apache Mesos abstracts CPU, memory, storage, and other compute resources away from machines (physical or virtual), enabling fault-tolerant and elastic distributed systems to easily be built and run effectively.
- [Scala: Marathon](https://mesosphere.github.io/marathon/): A cluster-wide init and control system for services in cgroups or Docker containers
- [Go: hashicorp/Nomad](https://github.com/hashicorp/nomad): Nomad is a cluster manager, designed for both long lived services and short lived batch processing workloads. Developers use a declarative job specification to submit work, and Nomad ensures constraints are satisfied and resource utilization is optimized by efficient task packing

## OS Configuration Management

- [Python: Ansible](http://www.ansible.com/): Deploy apps. Manage systems. Crush complexity. Ansible is a powerful automation tool that you can learn quickly.
- [Python: Fabric](http://www.fabfile.org/): Fabric is a Python (2.5-2.7) library and command-line tool for streamlining the use of SSH for application deployment or systems administration tasks.
- [Ruby: Puppet](http://puppetlabs.com/): IT Automation Software of System Administrators
- [Ruby: Capistrano](https://github.com/capistrano/capistrano): Capistrano is a framework for building automated deployment scripts. Although Capistrano itself is written in Ruby, it can easily be used to deploy projects of any language or framework, be it Rails, Java, or PHP.
- [Ruby: Chef](http://www.getchef.com/chef/): Infrastructure as Code
- [Python: SaltStack](http://saltstack.com/): SaltStack software orchestrates and automates the visualization, build and management of any legacy or modern infrastructure. SaltStack is known as the fastest, most scalable systems and configuration management software for CloudOps, ITOps and DevOps.
- [C: CFEngine](http://cfengine.com/): Lightweight agent system. Configuration state is specified via a declarative language.

## Terminal

- [Golang: termui](https://github.com/gizak/termui): Golang terminal dashboard
- [Golang: GoTTY](https://github.com/yudai/gotty): Share your terminal as a web application
- [Golang: s](https://github.com/zquestz/s): Open a web search in your terminal.


## Container

- Specification
    - [Open Containers Initiative](https://github.com/opencontainers)
- Container Linux
    - [Coreos](https://coreos.com/os/docs/latest/)
    - [RancherOS](http://rancher.com/rancher-os/)
	- [Operos](https://www.paxautoma.com/): Complete infrastructure and application management stack for commodity hardware.
- Container
    - [Docker](https://www.docker.com/open-source-0)
    - [rkt](https://coreos.com/rkt/)
        - https://coreos.com/rkt/docs/latest/getting-started-guide.html
    - [LXC/LXD](https://linuxcontainers.org/)
    - [Hyper](https://hypercontainer.io/)
- Container Registry
    - [Docker Distribution/Registry](https://github.com/docker/distribution): The Docker toolset to pack, ship, store, and deliver content. This repository's main product is the Docker Registry 2.0 implementation for storing and distributing Docker images. It supersedes the docker/docker-registry project with a new API design, focused around security and performance.
    - [Habor](https://github.com/vmware/harbor): An enterprise-class container registry server based on Docker Distribution
    - [Portus](http://port.us.org/): Authorization service and frontend for Docker registry (v2)
    - [$Quary](https://coreos.com/quay-enterprise/)
- Docker Cluster & Container Management Platform
    - [Kubernetes](http://kubernetes.io/)
        - [Helm](https://github.com/kubernetes/helm): The Kubernetes Package Manager
    - [Docker Swarm](https://docs.docker.com/engine/swarm/)
    - [Ali Pouch](https://github.com/alibaba/pouch)
    - [$Rancher 2.0](https://rancher.com/)
    - [$Tectonic](https://coreos.com/tectonic/)
- AI for Container
    - [Magalix](https://docs.magalix.cloud/v0.5): Magalix is the autopilot of the cloud.

## Virtualization

- [KVM](https://www.linux-kvm.org/page/Main_Page): KVM (for Kernel-based Virtual Machine) is a full virtualization solution for Linux on x86 hardware containing virtualization extensions (Intel VT or AMD-V). It consists of a loadable kernel module, kvm.ko, that provides the core virtualization infrastructure and a processor specific module, kvm-intel.ko or kvm-amd.ko.
- [QEMU](https://www.qemu.org/): QEMU is a generic and open source machine emulator and virtualizer.
- [xen](https://xenproject.org/): The official Xen Project member organizations include Alibaba  / Aliyun, AWS, AMD, Arm, Bitdefender, Cavium, Citrix, Huawei, Intel, Oracle, and Qualcomm.

## Serverless

- [Knative](https://github.com/knative/): Kubernetes-based platform to build, deploy, and manage modern serverless workloads
- [Go: fission](https://github.com/fission/fission): Fast Serverless Functions for Kubernetes
- [Go: OpenFaas](https://github.com/openfaas/faas): Open FaaS
- [Go: fn](https://github.com/fnproject/fn): The container native, cloud agnostic serverless platform.
- [Go: kubeless](https://github.com/kubeless/kubeless): Kubernetes Native Serverless Framework
- [Node: Serverless Framework](https://github.com/serverless/serverless)
- [Apache openwhisk](https://openwhisk.apache.org/)
- [Python: AppScale](https://github.com/AppScale/appscale): AppScale is an easy-to-manage serverless platform for building and running scalable web and mobile applications on any infrastructure. 

## Misc

- [vagrantup](https://www.vagrantup.com/): Create and configure lightweight, reproducible, and portable development environments.
- [Buildbot](http://docs.buildbot.net/current/index.html): Buildbot 是一个检查代码变化的自动化编译/ 测试的Python系统
- [tox](https://tox.readthedocs.io/en/latest/): tox aims to automate and standardize testing in Python. It is part of a larger vision of easing the packaging, testing and release process of Python software.
