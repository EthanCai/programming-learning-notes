<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [Project about DevOps](#project-about-devops)
	- [Code Repository](#code-repository)
	- [Code review](#code-review)
	- [Code Analysis and Metrics](#code-analysis-and-metrics)
	- [Scaffolding](#scaffolding)
	- [Build](#build)
	- [Continuous Integration](#continuous-integration)
	- [Bug/Issue Management](#bugissue-management)
	- [Unit Testing](#unit-testing)
	- [Database Testing](#database-testing)
	- [Database Management](#database-management)
	- [Automated Acceptance Testing/BDD](#automated-acceptance-testingbdd)
	- [Performance Testing](#performance-testing)
	- [System Monitor](#system-monitor)
	- [Process Supervisor](#process-supervisor)
	- [Deployment](#deployment)
	- [User Behavior Collection & Analysis](#user-behavior-collection-analysis)
	- [Infrastructure Management](#infrastructure-management)
	- [Automamtion](#automamtion)
	- [Static Websites Generator](#static-websites-generator)
	- [Misc](#misc)

<!-- /TOC -->

# Project about DevOps

## Code Repository

- [Git](http://www.git-scm.com/): Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
- [Gitlab](https://about.gitlab.com/): Open source git server
- [bonobo git server](https://bonobogitserver.com/): Simple git server for Windows. Set up your own self hosted git server on IIS for Windows. Manage users and have full control over your repositories with a nice user friendly graphical interface.
- [gitolite](https://github.com/sitaramc/gitolite): Hosting git repositories -- Gitolite allows you to setup git hosting on a central server, with very fine-grained access control and many (many!) more powerful features.


## Code review

- [Gerrit Code Review](https://www.gerritcodereview.com/): Gerrit provides web based code review and repository management for the Git version control system.


## Code Analysis and Metrics

- [ESlint](http://eslint.org/): The pluggable linting utility for JavaScript and JSX
    - [JSCS — JavaScript Code Style](http://jscs.info/): **JSCS has merged with ESLint!** JSCS is a code style linter and formatter for your style guide
- [SonarQube](http://www.sonarqube.org/): SonarQube is an open platform to manage code quality. As such, it covers the 7 axes of code quality:
- [StyleCop](https://stylecop.codeplex.com/) - StyleCop analyzes C# source code to enforce a set of style and consistency rules
- [FoxCop](https://msdn.microsoft.com/en-us/library/bb429476(v=vs.80).aspx) - FxCop is an application that analyzes managed code assemblies (code that targets the .NET Framework common language runtime) and reports information about the assemblies, such as possible design, localization, performance, and security improvements.
- [OpenCover](https://github.com/OpenCover/opencover): A code coverage tool for .NET 2 and above, support for 32 and 64 processes with both branch and sequence points; roots proudly based in PartCover


## Scaffolding

- [Yeoman](http://yeoman.io): The Yeoman workflow is comprised of three core tools for improving your productivity and satisfaction when building a web app.


## Build

- [Gradle](http://gradle.org/): OPEN SOURCE BUILD AUTOMATION. Get started with: Java / JVM | Android | Native (C / C++) | Web and many more!
- [Bazel](http://bazel.io/): Bazel is Google's own build tool, now publicly available in Beta. Bazel has built-in support for building both client and server software, including client applications for both Android and iOS platforms. It also provides an extensible framework that you can use to develop your own build rules.
- [Cmake](https://cmake.org/): CMake is an open-source, cross-platform family of tools designed to build, test and package software. CMake is used to control the software compilation process using simple platform and compiler independent configuration files, and generate native makefiles and workspaces that can be used in the compiler environment of your choice. The suite of CMake tools were created by Kitware in response to the need for a powerful, cross-platform build environment for open-source projects such as ITK and VTK.
- [Psake](https://github.com/psake/psake) - .NET-based build automation tool written in PowerShell
- [Invoke-Build](https://github.com/nightroman/Invoke-Build) - PowerShell build and test automation tool inspired by Psake.
- [MSBuild](https://github.com/Microsoft/msbuild) - The Microsoft Build Engine (MSBuild) is the build platform for .NET and Visual Studio
- [Wixtoolset](http://wixtoolset.org/): The WiX toolset builds Windows installation packages from XML source code. The toolset integrates seamlessly into build processes.


## Continuous Integration

- [CruiseControl.NET](http://www.cruisecontrolnet.org/) - an Automated Continuous Integration server, implemented using the .NET Framework
- [MyGet](http://www.myget.org/) - Continuous Integration and Deployment, Hosted Package Repository for NuGet, NPM, Bower and VSIX. [Free for OSS] [$]
- [Jenkins-CI](http://jenkins-ci.org/): An extensible open source continuous integration server
- [Go.cd](http://www.go.cd/): Automate and streamline the build-test-release cycle for worry-free, continuous delivery of your product.
- [janky](https://github.com/github/janky): Continuous integration server built on top of Jenkins and Hubot
- [Buildbot](http://buildbot.net/index.html): Python-based continuous integration testing framework; your pull requests are more than welcome!
- [teletraan](https://github.com/pinterest/teletraan): Teletraan is Pinterest's deploy system. It deploys hundreds of Pinterest internal services, supports tens of thousands hosts, and has been running in production for over a year.


## Bug/Issue Management

- [BugZilla](http://www.bugzilla.org/): Bugzilla is server software designed to help you manage software development.
- [Mantis Bug Tracker](http://www.mantisbt.org/index.php): MantisBT makes collaboration with team members & clients easy, fast, and professional
- [BugTracker.NET](http://ifdefined.com/bugtrackernet.html): BugTracker.NET is a free, open-source, web-based bug tracking and general purpose issue tracking application. It is in daily use by thousands of development, customer support, and help desk teams around the world.
- [BugNET](http://www.bugnetproject.com/): An open source issue tracking & project management application


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
- [Shouldly](https://github.com/shouldly/shouldly): Should testing for .net - the way Asserting *Should* be!


## Database Testing

- [dbUnit](http://dbunit.sourceforge.net/intro.html): database unit testing
- [TSQLT](http://tsqlt.org/): tSQLt is a database unit testing framework for Microsoft SQL Server. tSQLt is compatible with SQL Server 2005 (service pack 2 required) and above on all editions.
- [DbFit](http://dbfit.github.io/dbfit/index.html): Test-driven database development. Write readable, easy-to-maintain unit and integration tests for your database code.


## Database Management

- [SqlPad](http://rickbergfalk.github.io/sqlpad/): Run SQL in your browser...Supports Postgres, MySQL, SQL Server and Vertica.
- [sqitch](http://sqitch.org/): Sqitch is a database change management application.


## Automated Acceptance Testing/BDD

- [fitnesse](http://www.fitnesse.org/FrontPage): The fully integrated standalone wiki and acceptance testing framework
- [Cumuber](https://cucumber.io/): Cucumber is a software tool that computer programmers use for testing other software. It runs automated acceptance tests written in a behavior-driven development (BDD) style.
    - [cucumber.js](https://github.com/cucumber/cucumber-js): Cucumber, the popular Behaviour-Driven Development tool, brought to your JavaScript stack.It runs on both Node.js and modern web browsers.
- [SpecFlow](http://www.specflow.org/): SpecFlow aims at bridging the communication gap between domain experts and developers by binding business readable behavior specifications and examples to the underlying implementation.
- [Selenium](http://www.seleniumhq.org/): Selenium is a suite of tools to automate web browsers across many platforms.
- [ROBOT FRAMEWORK](http://robotframework.org/): Robot Framework is a generic test automation framework for acceptance testing and acceptance test-driven development (ATDD).
- [JBehave](http://jbehave.org): JBehave is a framework for Behaviour-Driven Development (BDD). BDD is an evolution of test-driven development (TDD) and acceptance-test driven design, and is intended to make these practices more accessible and intuitive to newcomers and experts alike. It shifts the vocabulary from being test-based to behaviour-based, and positions itself as a design philosophy.
- [Jasmine](https://github.com/jasmine/jasmine): Jasmine is a Behavior Driven Development testing framework for JavaScript. It does not rely on browsers, DOM, or any JavaScript framework. Thus it's suited for websites, Node.js projects, or anywhere that JavaScript can run.


## Performance Testing

- [Go: Gor](https://github.com/buger/gor): Gor is a simple http traffic replication tool written in Go. Its main goal is to replay traffic from production servers to staging and dev environments.
- [Web Bench](http://home.tiscali.cz:8080/~cz210552/webbench.html): Web Bench是一个简单的web或者web代理服务的基准测试工具。（它）使用fork()模拟多个客户端并且可以发起HTTP/0/9-HTTP/1.1的请求。这个基准测试不是非常符合实际情况，但是可以测试出你的HTTP服务是否可以处理多个客户同时访问而不会把你的机器弄挂掉。这个工具可以获得服务的两个指标：每分钟响应请求数量（pages/min）和每秒钟传输数据量（bytes/sec）。
- [Siege](https://www.joedog.org/siege-home/): Siege（英文意思是围攻）是一个压力测试和评测工具，设计用于WEB开发这评估应用在压力下的承受能力：可以根据配置对一个WEB站点进行多用户的并发访问，记录每个用户所有请求过程的相应时间，并在一定数量的并发访问下重复进行。 Siege 支持基本的认证，cookies， HTTP 和 HTTPS 协议。
- [ab - Apache HTTP server benchmarking tool](http://jmeter.apache.org/): ab命令会创建很多的并发访问线程，模拟多个访问者同时对某一URL地址进行访问。它的测试目标是基于URL的，因此，既可以用来测试Apache的负载压力，也可以测试nginx、lighthttp、tomcat、IIS等其它Web服务器的压力。ab命令对发出负载的计算机要求很低，既不会占用很高CPU，也不会占用很多内存，但却会给目标服务器造成巨大的负载，其原理类似CC攻击。
- [TCPCopy](https://github.com/session-replay-tools/tcpcopy): TCPCopy is a TCP stream replay tool to support real testing of Internet server applications.
- [Apache JMeter](http://jmeter.apache.org/): Apache JMeter是一个专门为运行和服务器装载测试而设计的、100％的纯Java桌面运行程序。原先它是为Web/HTTP测试而设计的，但是它已经扩展以支持各种各样的测试模块。它和用于HTTP和SQL数据库（使用JDBC）的模块一起运送。它可以用来测试静止资料库或者活动资料库中的服务器的运行情况，可以用来模拟对服务器或者网络系统加以重负荷以测试它的抵抗力，或者用来分析不同负荷类型下的所有运行情况。它也提供了一个可替换的界面用来定制数据显示，测试同步及测试的创建和执行。
    - [Badboy](http://www.badboy.com.au/): Badboy is a powerful tool designed to aid in testing and development of complex dynamic applications. Badboy makes web testing and development easier with dozens of features including a simple yet comprehensive capture/replay interface, powerful load testing support, detailed reports, graphs and much more!
    - [ruby-jmeter](https://github.com/flood-io/ruby-jmeter): A Ruby based DSL for building JMeter test plans
- [Gatling](http://gatling.io/): Gatling is an open-source load testing framework based on Scala, Akka and Netty
- [West Wind Websurge](http://websurge.west-wind.com/): We believe that testing HTTP requests and load testing a site should be easy - something that takes a few minutes to set up and then runs on a regular basis during the development process, so that you can monitor performance of your site while you are building it. To this end we built West Wind WebSurge with the developer and testers in mind to make it easy to create HTTP requests or entire sessions, and then easily play back either individual URLs for development response testing, or for full-on testing under heavy load. Sessions are stored in plain text files so that they can be easily stored with projects or shared via source control for all users to have access.
- [Go: toxy](https://github.com/h2non/toxy): Hackable HTTP proxy to simulate server failure scenarios and unexpected network conditions
- [tcpkali](https://github.com/machinezone/tcpkali): Fast multi-core TCP and WebSockets load generator.


## System Monitor

- [Nagios](https://www.nagios.org/): Nagios Is The Industry Standard In IT Infrastructure Monitoring. Achieve instant awareness of IT infrastructure problems, so downtime doesn't adversely affect your business.
- [icinga](https://www.icinga.org/): ICINGA项目是 由Michael Luebben、HendrikB?cker和JoergLinge等人发起的，他们都是现有的Nagios项目社区委员会的成员，他们承诺，新的开源项 目将完全兼容以前的Nagios应用程序及扩展功能。在新项目的网站上，他们是如此定义ICINGA的，这将是一个介于Nagios社区版和企业版间的产 品。特别将致力于解决Nagios项目现在的问题，比如不能及时处理Nagios项目的bug、新功能不能及时添加等。还有在新的ICINGA项目中，将 更好的实现数据库集成方面的功能，标准化第三发应用程序的接口等。
- [Zabbix](http://www.zabbix.com/): Zabbix is the ultimate enterprise-level software designed for real-time monitoring of millions of metrics collected from tens of thousands of servers, virtual machines and network devices.
- [Opserver](https://github.com/opserver/opserver): Opserver is a monitoring system by the team at Stack Exchange, home of Stack Overflow.
- [Ganglia Monitoring System](http://ganglia.info/): Ganglia is a scalable distributed monitoring system for high-performance computing systems such as clusters and Grids. It is based on a hierarchical design targeted at federations of clusters. It leverages widely used technologies such as XML for data representation, XDR for compact, portable data transport, and RRDtool for data storage and visualization. It uses carefully engineered data structures and algorithms to achieve very low per-node overheads and high concurrency. The implementation is robust, has been ported to an extensive set of operating systems and processor architectures, and is currently in use on thousands of clusters around the world. It has been used to link clusters across university campuses and around the world and can scale to handle clusters with 2000 nodes.
- [Tsar](https://github.com/kongjian/tsar): Tsar (Taobao System Activity Reporter) is a monitoring tool, which can be used to gather and summarize system information, e.g. CPU, load, IO, and application information, e.g. nginx, HAProxy, Squid, etc. The results can be stored at local disk or sent to Nagios.
- [collectd](http://collectd.org/): collectd is a daemon which collects system performance statistics periodically and provides mechanisms to store the values in a variety of ways, for example in RRD files.
- [osquery](https://github.com/facebook/osquery): SQL powered operating system instrumentation, monitoring, and analytics.
- [Graphite - Scalable Realtime Graphing](http://graphite.wikidot.com/): Graphite 是一个用于采集网站实时信息并进行统计的开源项目，可用于采集多种网站服务运行状态信息。Graphite服务平均每分钟有4800次更新操作。实践已经证实要监测网站发发生什么是非常有用的，它的简单文本协议和绘图功能可以方便地即插即 用的方式用于任何需要监控的系统上。
- [Go: Prometheus](http://prometheus.io/): An open-source service monitoring system and time series database.
- [Go: bosun](https://github.com/bosun-monitor/bosun): Bosun is an open-source, MIT licensed, monitoring and alerting system by Stack Exchange. It has an expressive domain specific language for evaluating alerts and creating detailed notifications. It also lets you test your alerts against history for a faster development experience.
- [Open-Falcon企业级监控系统解决方案](http://open-falcon.com/): Open-Falcon 是小米运维部开源的一款互联网企业级监控系统解决方案.

## Process Supervisor

- [Supervisor](http://supervisord.org): Supervisor is a client/server system that allows its users to control a number of processes on UNIX-like operating systems.
- [PM2](https://github.com/Unitech/pm2): Production process manager for Node.js applications with a built-in load balancer https://app.keymetrics.io/


## Deployment

- [Unfold](https://github.com/thomasvm/unfold) - Powershell-based deployment solution for .net web applications


## User Behavior Collection & Analysis

- [Piwik - Open Analytics Platform](http://piwik.org/): Piwik is an open analytics platform currently used by individuals, companies and governments all over the world. With Piwik, your data will always be yours. Learn why Piwik is the right web analytics tool for you below.
- [Open Web Analytics](http://www.openwebanalytics.com/): Open Web Analytics (OWA) is open source web analytics software that you can use to track and analyze how people use your websites and applications. OWA is licensed under GPL and provides website owners and developers with easy ways to add web analytics to their sites using simple Javascript, PHP, or REST based APIs.
- [Snowplow - the event analytics platform](http://snowplowanalytics.com/): Have every single event, from your websites, mobile apps, desktop applications and server-side systems, stored in your own data warehouse and available to action in real-time.
- [tracking.js](http://trackingjs.com/): The tracking.js library brings different computer vision algorithms and techniques into the browser environment. By using modern HTML5 specifications, we enable you to do real-time color tracking, face detection and much more — all that with a lightweight core (~7 KB) and intuitive interface.


## Infrastructure Management

- [Apache Mesos](http://mesos.apache.org/): Apache Mesos abstracts CPU, memory, storage, and other compute resources away from machines (physical or virtual), enabling fault-tolerant and elastic distributed systems to easily be built and run effectively.
- [Marathon](https://mesosphere.github.io/marathon/): A cluster-wide init and control system for services in cgroups or Docker containers
- [Chronos](http://mesos.github.io/chronos/): Chronos is Airbnb's replacement for cron. It is a distributed and fault-tolerant scheduler that runs on top of Apache Mesos that can be used for job orchestration. It supports custom Mesos executors as well as the default command executor. Thus by default, Chronos executes sh (on most systems bash) scripts.


## Automamtion

- [Chef](http://www.getchef.com/chef/): Infrastructure as Code
- [Ansible](http://www.ansible.com/): Deploy apps. Manage systems. Crush complexity. Ansible is a powerful automation tool that you can learn quickly.
- [Puppet](http://puppetlabs.com/): IT Automation Software of System Administrators
- [SaltStack](http://saltstack.com/): SaltStack software orchestrates and automates the visualization, build and management of any legacy or modern infrastructure. SaltStack is known as the fastest, most scalable systems and configuration management software for CloudOps, ITOps and DevOps.
- [cfengine](http://cfengine.com/): Lightweight agent system. Configuration state is specified via a declarative language.


## Misc

- [twill](http://twill.idyll.org/): a simple scripting language for Web browsing
- [vagrantup](https://www.vagrantup.com/): Create and configure lightweight, reproducible, and portable development environments.
- [hubot](https://hubot.github.com/): GitHub, Inc., wrote the first version of Hubot to automate our company chat room. Hubot knew how to deploy the site, automate a lot of tasks, and be a source of fun in the company. Eventually he grew to become a formidable force in GitHub. But he led a private, messy life. So we rewrote him.
