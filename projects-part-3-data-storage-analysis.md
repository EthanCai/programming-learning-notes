- [Projects about Data Storage and Analysis](#projects-about-data-storage-and-analysis)
  - [Database and Caching Platform](#database-and-caching-platform)
  - [Database](#database)
  - [Memory Database](#memory-database)
  - [Graph Database](#graph-database)
  - [Database Engine](#database-engine)
  - [NoSQL Database](#nosql-database)
  - [Time Series Database](#time-series-database)
  - [JSON Storage](#json-storage)
  - [OLAP - Data Warehouse](#olap---data-warehouse)
  - [Search](#search)
  - [Text Processing](#text-processing)
  - [Crawler](#crawler)
  - [Recommender System](#recommender-system)
  - [Big Data](#big-data)
  - [Distributed Realtime Computation System](#distributed-realtime-computation-system)
  - [Data Visualization](#data-visualization)
  - [Workflow System](#workflow-system)
  - [Log Process](#log-process)
  - [Notebook](#notebook)


# Projects about Data Storage and Analysis

## Database and Caching Platform

- [Apache Ignite](https://ignite.apache.org/): Apache Ignite In-Memory Data Fabric is a high-performance, integrated and distributed in-memory platform for computing and transacting on large-scale data sets in real-time, orders of magnitude faster than possible with traditional disk-based or flash technologies.


## Database

- [SQL Server](https://msdn.microsoft.com/en-us/library/bb545450.aspx)
- [PostgreSQL](http://www.postgresql.org/):
    - [pgAdmin](https://www.pgadmin.org/)
    - [PostGIS](http://postgis.refractions.net): PostGIS在对象关系型数据库PostgreSQL上增加了存储管理空间数据的能力，相当于Oracle的spatial部分。PostGIS最大的特点是符合并且实现了OpenGIS的一些规范，是最著名的开源GIS数据库。
    - [PgBouncer](https://pgbouncer.github.io/): Lightweight connection pooler for PostgreSQL
    - [pgtool](http://www.pgpool.net/): Pgpool-II is a middleware that works between PostgreSQL servers and a PostgreSQL database client.
    - [pgmetrics](https://pgmetrics.io/): Easily collect and report PostgreSQL metrics for scripting, automation and troubleshooting.
    - [Postgres-XL](https://www.postgres-xl.org/overview/): Postgres-XL is a horizontally scalable open source SQL database cluster, flexible enough to handle varying database workloads
    - [Citus](https://github.com/citusdata/citus): Scalable PostgreSQL for multi-tenant and real-time workloads
    - [2ndquadrant](https://www.2ndquadrant.com/en/books/): Your diligent team of PostgreSQL experts
- [MySQL](http://www.mysql.com/)
    - [MariaDB](http://mariadb.org/)
    - [WebScaleSQL](http://webscalesql.org/)
- Distributed Database
    - [Tidb](https://github.com/pingcap/tidb): TiDB is a distributed NewSQL database compatible with MySQL protocol
    - [CockroachDB](https://www.cockroachlabs.com/product/cockroachdb/)
    - [FoundationDB](https://www.foundationdb.org/)
    - [DynomiteDB](http://www.dynomitedb.com/): A high performance, linearly scalable, highly available (HA) and distributed open-source database with support for pluggable persistent and in-memory storage engines.
- [RocksDB](http://rocksdb.org/): The RocksDB library provides a persistent key value store. Keys and values are arbitrary byte arrays. The keys are ordered within the key value store according to a user-specified comparator function.
	- [MyRocks](http://myrocks.io/): A RocksDB storage engine with MySQL
- [noms](https://github.com/attic-labs/noms): The versioned, forkable, syncable database. Noms is a decentralized database based on ideas from Git.

## Memory Database

- [SQLlite](http://www.sqlite.org/index.html)
- [LMDB](https://github.com/clibs/lmdb): Symas Lightning Memory-Mapped Database
- [Apache GEODE](http://geode.apache.org/): Geode is an open source , distributed, in-memory database for scale-out applications.

## Graph Database

- [Cayley](https://github.com/cayleygraph/cayley): Cayley is an open-source graph inspired by the graph database behind Freebase and Google's Knowledge Graph.
- [Dgraph](https://dgraph.io/): distributed graph database
- [JanusGraph](https://janusgraph.org/): Distributed, open source, massively scalable graph database
- [Neo4j](http://neo4j.com): Neo4j is an open-source NoSQL graph database implemented in Java and Scala.
- [ArangoDB](https://www.arangodb.com/): Natively store data for graph, document and search needs.Utilize feature-rich access with one query language.
- [GraphView](https://github.com/Microsoft/GraphView): GraphView is a DLL library that enables users to use SQL Server or Azure SQL Database to manage graphs. It connects to a SQL database locally or in the cloud, stores graph data in tables and queries graphs through a SQL-extended language. It is not an independent database, but a middleware that accepts graph operations and translates them to T-SQL executed in SQL Server or Azure SQL Database.

## Database Engine

- [InnoDB](https://en.wikipedia.org/wiki/InnoDB): InnoDB is a storage engine for MySQL. MySQL 5.5 and later use it by default.[1] It provides the standard ACID-compliant transaction features, along with foreign key support (Declarative Referential Integrity).
- [XtraDB](https://en.wikipedia.org/wiki/XtraDB): Percona XtraDB is a storage engine for the MariaDB and Percona Server databases, and is intended as a drop-in replacement to InnoDB, which is one of the default engines available on the MySQL database.
- [Berkerly DB](http://www.oracle.com/technetwork/database/database-technologies/berkeleydb/overview/index.html): 介绍见[这里](https://en.wikipedia.org/wiki/Berkeley_DB)
- [Tokyo Cabinet](http://fallabs.com/tokyocabinet/): Tokyo Cabinet is a library of routines for managing a database. The database is a simple data file containing records, each is a pair of a key and a value. Every key and value is serial bytes with variable length. Both binary data and character string can be used as a key and a value. There is neither concept of data tables nor data types. Records are organized in hash table, B+ tree, or fixed-length array.

## NoSQL Database

- [MongoDB](https://www.mongodb.org/)
- [RethinkDB](https://www.rethinkdb.com/)
- [TokuMX](http://www.tokutek.com/): High-Performance MongoDB
- [RavenDB](http://ravendb.net/): A linq enabled document database for .NET
- [EventStore](https://github.com/EventStore/EventStore): The open-source, functional database with Complex Event Processing in JavaScript.
- [LevelDB](https://github.com/google/leveldb): LevelDB is a fast key-value storage library written at Google that provides an ordered mapping from string keys to string values.
    - [eLevelDB](https://github.com/basho/eleveldb): eLevelDB 是一个 Erlang 应用程序，封装了 LevelDB
- [Cassandra](http://cassandra.apache.org/): The Apache Cassandra database is the right choice when you need scalability and high availability without compromising performance. Linear scalability and proven fault-tolerance on commodity hardware or cloud infrastructure make it the perfect platform for mission-critical data. Cassandra's support for replicating across multiple datacenters is best-in-class, providing lower latency for your users and the peace of mind of knowing that you can survive regional outages.
- [ScyllaDB](https://github.com/scylladb/scylla): NoSQL data store using the seastar framework, compatible with Apache Cassandra
- [GridDB](https://griddb.net/en/): GridDB is an In-Memory NoSQL Database for highly scalable IoT applications

## Time Series Database

- [Go: Prometheus](http://prometheus.io/): An open-source service monitoring system and time series database.
- [Apache IoTDB](https://iotdb.apache.org/#/): Apache IoTDB (incubating) (Database for Internet of Things) is an integrated data management engine designed for timeseries data. It provides users with services for data collection, storage and analysis. 
- [Timescaledb](https://github.com/timescale/timescaledb): TimescaleDB is an open-source database designed to make SQL scalable for time-series data. It is engineered up from PostgreSQL, providing automatic partitioning across time and space (partitioning key), as well as full SQL support.
- [PipelineDB](https://www.pipelinedb.com/): High-performance time-series aggregation for PostgreSQL. An open-source PostgreSQL extension that runs SQL queries continuously on streams, incrementally storing results in tables.
- InfluxData Open Source Platform
    - [Telegraf](https://github.com/influxdata/telegraf): The plugin-driven server agent for collecting & reporting metrics.
    - [InfluxDB](https://github.com/influxdata/influxdb): Scalable datastore for metrics, events, and real-time analytics
    - [Chronograf](https://github.com/influxdata/chronograf): Chronograf is an open-source web application written in Go and React.js that provides the tools to visualize your monitoring data and easily create alerting and automation rule
    - [Kapacitor](https://github.com/influxdata/kapacitor): Open source framework for processing, monitoring, and alerting on time series data
- [Riak TS](http://basho.com/products/riak-ts/)
- [TDengine](https://github.com/taosdata/TDengine): An open-source big data platform designed and optimized for the Internet of Things (IoT).

reference:

- [InfluxData Platform](https://www.influxdata.com/products/editions/)
    - [Open Source Time Series Platform](https://www.influxdata.com/time-series-platform/)
- [Time Series Database](https://www.influxdata.com/time-series-database/)

## JSON Storage

- [Kinto](https://github.com/Kinto/kinto): Kinto is a lightweight JSON storage service with synchronisation and sharing abilities. It is meant to be easy to use and easy to self-host.

## OLAP - Data Warehouse

- [ClickHouse](https://clickhouse.tech/): ClickHouse is a fast open-source OLAP database management system
- [facebook presto](https://prestodb.io/): Presto is an open source distributed SQL query engine for running interactive analytic queries against data sources of all sizes ranging from gigabytes to petabytes.
- [Greenplum Database](http://greenplum.org): Greenplum DB 号称是世界上第一个开源的大规模并行数据仓库，最初是基于 PostgreSQL，现在已经添加了大量数据库方面的创新。Greenplum 提供 PD 级别数据量的强大和快速分析能力，特别是面向大数据方面的分析能力，支持大数据的超高性能分析查询。
- [druid](http://druid.io/druid.html): Druid is an open-source data store designed for sub-second queries on real-time and historical data. It is primarily used for business intelligence (OLAP) queries on event data. Druid provides low latency (real-time) data ingestion, flexible data exploration, and fast data aggregation. Existing Druid deployments have scaled to trillions of events and petabytes of data. Druid is most commonly used to power user-facing analytic applications.
- [Infobright community edition](https://www.infobright.com/): [下载地址](https://github.com/JonGates/infobright)
- [Pinot](https://github.com/linkedin/pinot): Pinot is a realtime distributed OLAP datastore, which is used at LinkedIn to deliver scalable real time analytics with low latency. It can ingest data from offline data sources (such as Hadoop and flat files) as well as online sources (such as Kafka). Pinot is designed to scale horizontally.

## Search

- [Java: Apache Lucene](http://lucene.apache.org/core/index.html): Apache LuceneTM is a high-performance, full-featured text search engine library written entirely in Java. It is a technology suitable for nearly any application that requires full-text search, especially cross-platform.
  - [C++: Lucene++](https://github.com/luceneplusplus/LucenePlusPlus): Lucene++ is an up to date C++ port of the popular Java Lucene library, a high-performance, full-featured text search engine.
  - [Go: golucene](https://github.com/balzaczyy/golucene): Go (Golang) port of Apache Lucene
- [Java: Apache Solr](http://lucene.apache.org/solr/): Solr is the popular, blazing-fast, open source enterprise search platform built on Apache Lucene.
    - [mmseg4j-solr](https://github.com/chenlb/mmseg4j-solr): mmseg4j for lucene or solr analyzer
    - [mmseg4j-core](https://github.com/chenlb/mmseg4j-core): mmseg4j core MMSEG for java chinese analyzer
- [Java: ElasticSearch](https://www.elastic.co/): elasticsearch 的目标是解决上面的所有问题以及更多。她是开源的（Apache2协议），分布式的，RESTful的，构建在Apache Lucene之上的的搜索引擎.
    - [elasticsearch-rtf](https://github.com/medcl/elasticsearch-rtf): elasticsearch中文发行版，针对中文集成了相关插件，并带有Demo，方便新手学习,或者在生产环境中直接使用
    - [elasticsearch-analysis-ik](https://github.com/medcl/elasticsearch-analysis-ik): The IK Analysis plugin integrates Lucene IK analyzer into elasticsearch, support customized dictionary.
    - [elasticsearch-analysis-mmseg](https://github.com/medcl/elasticsearch-analysis-mmseg): Mmseg Analysis for ElasticSearch
    - [elasticsearch-analysis-pinyin](https://github.com/medcl/elasticsearch-analysis-pinyin): The Pinyin Analysis plugin integrates Pinyin4j(http://pinyin4j.sourceforge.net/) module into elasticsearch.
- [C++: Sphinx](http://sphinxsearch.com/): Sphinx Search 是由俄罗斯人Andrew Aksyonoff 开发的高性能全文搜索软件包，在GPL与商业协议双许可协议下发行。Sphinx is an open source full text search server, designed from the ground up with performance, relevance (aka search quality), and integration simplicity in mind. It's written in C++ and works on Linux (RedHat, Ubuntu, etc), Windows, MacOS, Solaris, FreeBSD, and a few other systems.
    - [sphinx-for-chinese](http://sphinx-search.com/): sphinx-for-chinese是一款专注于中文搜索的全文检索软件，在sphinx的基础上添加了中文处理模块并优化了中文搜索效果。
- [C++: xunsearch](http://www.xunsearch.com/): 开源免费、高性能、多功能, 简单易用的专业全文检索技术方案
- Ego
    - [Golang: gse](https://github.com/go-ego/gse): Go efficient text segmentation; support english, chinese, japanese and other. Go 语言高性能分词
    - [Golang: riot](https://github.com/go-ego/riot): Go Open Source, Distributed, Simple and efficient Search Engine
    - [Golang: bleve](https://github.com/blevesearch/bleve): A modern text indexing library for go

**Code Search**

- [OpenGrok](http://opengrok.github.io/OpenGrok/): OpenGrok is a fast and usable source code search and cross reference engine.
- [Hound](https://github.com/etsy/hound): Hound is an extremely fast source code search engine.
- [zoekt](https://github.com/google/zoekt): Fast trigram based code search
- [Google code search](https://github.com/google/codesearch): Code Search is a tool for indexing and then performing regular expression searches over large bodies of source code. It is a set of command-line programs written in Go.

## Text Processing

- [Golang: sego](https://github.com/huichen/sego): Go中文分词
- [Golang: gse](https://github.com/go-ego/gse): Go efficient text segmentation; support english, chinese, japanese and other.
- [Golang: prose](https://github.com/jdkato/prose): A Golang library for text processing, including tokenization, part-of-speech tagging, and named-entity extraction.
- [Golang: gpy](https://github.com/go-ego/gpy): Go 语言汉字转拼音工具

- [Golang: goquery](https://github.com/PuerkitoBio/goquery): goquery brings a syntax and a set of features similar to jQuery to the Go language. It is based on Go's net/html package and the CSS Selector library cascadia. Since the net/html parser returns nodes, and not a full-featured DOM tree, jQuery's stateful manipulation functions (like height(), css(), detach()) have been left off.
- [Java: Apache Tika](http://tika.apache.org/): The Apache Tika™ toolkit detects and extracts metadata and text from over a thousand different file types (such as PPT, XLS, and PDF). All of these file types can be parsed through a single interface, making Tika useful for search engine indexing, content analysis, translation, and much more.
- [.NET: Toxy - .NET Text/Data Extraction Framework](https://toxy.codeplex.com): Toxy is a .NET data/text extraction framework similar to Apache Tika in Java. It supports a lot of popular formats such as docx, xlsx, xls, pdf, csv, txt, epub, html and so on.
- [.NET: Rant2](https://github.com/TheBerkin/Rant): Rant is an all-purpose procedural text engine that is most simply described as the opposite of Regex. It has been refined to include a dizzying array of features for handling everything from the most basic of string generation tasks to advanced dialogue generation, code templating, automatic formatting, and more.

## Crawler

参考：https://github.com/BruceDone/awesome-crawler

- [Golang: Pholcus](https://github.com/henrylee2cn/pholcus): Pholcus（幽灵蛛）是一款纯Go语言编写的高并发、分布式、重量级爬虫软件，支持单机、服务端、客户端三种运行模式，拥有Web、GUI、命令行三种操作界面；规则简单灵活、批量任务并发、输出方式丰富（mysql/mongodb/csv/excel等）、有大量Demo共享；同时她还支持横纵向两种抓取模式，支持模拟登录和任务暂停、取消等一系列高级功能
- [Golang: Colly](http://go-colly.org/): Fast and Elegant Scraping Framework for Gophers
- [Java: Apache Nutch](http://nutch.apache.org/): Apache Nutch是一个用Java编写的开源网络爬虫。Apache Nutch对于Solr已经支持得很好，这大大简化了Nutch与Solr的整合。
    - [Java: yahoo/anthelion](https://github.com/yahoo/anthelion): Anthelion is a Nutch plugin for focused crawling of semantic data. The project is an open-source project released under the Apache License 2.0.
- [Python: Scrapy](https://scrapy.org/): An open source and collaborative framework for extracting the data you need from websites.
In a fast, simple, yet extensible way.
- [Java: Norconex HTTP Collector](http://www.norconex.com/collectors/collector-http/): Open-Source Enterprise Web Crawler
- [Java: heritrix3](https://github.com/internetarchive/heritrix3): Heritrix is the Internet Archive's open-source, extensible, web-scale, archival-quality web crawler project.

## Recommender System

- [SUGGEST: Recommendation Engine](http://glaros.dtc.umn.edu/gkhome/suggest/overview): SUGGEST is a Top-N recommendation engine that implements a variety of recommendation algorithms. Top-N recommender systems, a personalized information filtering technology, are used to identify a set of N items that will be of interest to a certain user. In recent years, top-N recommender systems have been used in a number of different applications such to recommend products a customer will most likely buy; recommend movies, TV programs, or music a user will find enjoyable; identify web-pages that will be of interest; or even suggest alternate ways of searching for information.
- [easyrec](http://easyrec.org/): With the open source recommendation engine easyrec you can add recommendations to your website within minutes. easyrec is a web application written in Java that provides personalized recommendations using RESTful Web Services ready to be integrated in your web enabled applications.
- [MyMediaLite](https://github.com/zenogantner/MyMediaLite): recommender system library for the CLR (.NET)
- [LensKit](http://lenskit.org/): Open-Source Tools for Recommender Systems
- [Crab](http://muricoca.github.io/crab/): A Recommender Framework in Python

## Big Data

- [Hadoop and related projects](http://hadoop.apache.org/)
    - [**Common**](http://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-common/CLIMiniCluster.html): The common utilities that support the other Hadoop modules.
    - [**HDFS**](http://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/HdfsUserGuide.html): A distributed file system that provides high-throughput access to application data.
    - [**YARN**](http://hadoop.apache.org/docs/current/hadoop-yarn/hadoop-yarn-site/YARN.html): A framework for job scheduling and cluster resource management.
    - [**MapReduce**](http://hadoop.apache.org/docs/current/hadoop-mapreduce-client/hadoop-mapreduce-client-core/MapReduceTutorial.html): A YARN-based system for parallel processing of large data sets.
- [Apache Spark](http://spark.apache.org/): a fast and general engine for large-scale data processing
    - [Apache Livy](https://livy.apache.org/): A REST Service for Apache Spark
- [Apache TAJO](http://tajo.apache.org/): A big data warehouse system on Hadoop
- [Apache Kylin](http://kylin.incubator.apache.org/): Apache Kylin is an open source Distributed Analytics Engine from eBay Inc. that provides SQL interface and multi-dimensional analysis (OLAP) on Hadoop supporting extremely large datasets
- [Apache Hive](http://hive.apache.org/): The Apache Hive ™ data warehouse software facilitates querying and managing large datasets residing in distributed storage. Hive provides a mechanism to project structure onto this data and query the data using a SQL-like language called HiveQL. At the same time this language also allows traditional map/reduce programmers to plug in their custom mappers and reducers when it is inconvenient or inefficient to express this logic in HiveQL.
- [Apache HBase](http://hbase.apache.org/): Apache HBase™ is the Hadoop database, a distributed, scalable, big data store
- [Apache HAWQ](http://hawq.incubator.apache.org): HAWQ 是 Pivotal 设计的一个大规模并行 SQL 分析处理引擎，支持事务处理。HAWQ 将复杂的查询分割成简单的任何，并分发到并行处理系统中的处理单元执行。包括查询规划器、动态管道、前沿互联和查询执行优化器等等。提供最高级别的性能和可伸缩性。HAWQ 基于 Hadoop 架构。
- [Go: Pachyderm](https://github.com/pachyderm/pachyderm): Pachyderm is a software platform the supports the storage and processing of large data sets. Pachyderm is inspired by the Hadoop ecosystem but shares no code with it. Instead, we leverage the container ecosystem to provide the broad functionality of Hadoop with the ease of use of Docker.
- [Pony: Wallaroo](https://www.wallaroolabs.com/): The ultrafast and elastic data processing engine.
- [Apache Calcite](https://calcite.apache.org/): The foundation for your next high-performance database.

## Distributed Realtime Computation System

- [Apache Storm](http://storm.apache.org/): Storm has many use cases: realtime analytics, online machine learning, continuous computation, distributed RPC, ETL, and more. Storm is fast: a benchmark clocked it at over a million tuples processed per second per node. It is scalable, fault-tolerant, guarantees your data will be processed, and is easy to set up and operate.
    - [jstorm](https://github.com/alibaba/jstorm): JStorm is a distributed and fault-tolerant realtime computation system. Inspired by Apache Storm, JStorm has been completely rewritten in Java and provides many more enhanced features. JStorm has been widely used in many enterprise environments and proved robust and stable.
- [Twitter Heron](http://dl.acm.org/citation.cfm?id=2742788): 参考[Twitter发布新的大数据实时分析系统Heron](http://geek.csdn.net/news/detail/33750)
- [Apache Samza](http://samza.apache.org/): Apache Samza is a distributed stream processing framework. It uses Apache Kafka for messaging, and Apache Hadoop YARN to provide fault tolerance, processor isolation, security, and resource management.
- [Apache Flink](http://flink.apache.org/): Apache Flink is an open source platform for scalable batch and stream data processing.
- [Data Sketches](https://datasketches.github.io): A Java software library of stochastic(随机的) streaming algorithms

## Data Visualization

- [Apache Zeppelin](http://www.zepl.com/): A web-based notebook that enables interactive data analytics. You can make beautiful data-driven, interactive and collaborative documents with SQL, Scala and more.
- [Kibana](https://www.elastic.co/products/kibana): Kibana 是一个为 Logstash 和 ElasticSearch 提供的日志分析的 Web 接口。可使用它对日志进行高效的搜索、可视化、分析等各种操作

## Workflow System

- [Python: Airflow](https://github.com/airbnb/airflow): a workflow management platform
- [Python: Perfect](https://github.com/PrefectHQ/prefect): Prefect is a new workflow management system, designed for modern infrastructure and powered by the open-source Prefect Core workflow engine. Users organize Tasks into Flows, and Prefect takes care of the rest.
- [Java: Azkaban](https://azkaban.github.io/): Azkaban is a batch workflow job scheduler created at LinkedIn to run Hadoop jobs. Azkaban resolves the ordering through job dependencies and provides an easy to use web user interface to maintain and track your workflows.
- [Java: Rundeck](http://rundeck.org/index.html): job scheduler and runbook automation
- [Go: Argo](https://github.com/argoproj/argo): Argo Workflows is an open source container-native workflow engine for orchestrating parallel jobs on Kubernetes. Argo Workflows is implemented as a Kubernetes CRD (Custom Resource Definition).

Library:

- [Go: SciPipe](https://github.com/scipipe/scipipe): SciPipe is a library for writing Scientific Workflows, sometimes also called "pipelines", in the Go programming language.
- [Python: luigi](https://github.com/spotify/luigi): Luigi is a Python module that helps you build complex pipelines of batch jobs. It handles dependency resolution, workflow management, visualization etc. It also comes with Hadoop support built in.
- [dotNET: Workflow-core](https://github.com/danielgerlag/workflow-core): Lightweight workflow engine for .NET Standard

Common Workflow Language:

- [Common Workflow Language](https://www.commonwl.org/): The Common Workflow Language (CWL) is a specification for describing analysis workflows and tools in a way that makes them portable and scalable across a variety of software and hardware environments, from workstations to cluster, cloud, and high performance computing (HPC) environments. CWL is designed to meet the needs of data-intensive science, such as Bioinformatics, Medical Imaging, Astronomy, Physics, and Chemistry.


## Log Process

- [Apache Flume](http://flume.apache.org/): Flume is a distributed, reliable, and available service for efficiently collecting, aggregating, and moving large amounts of log data. It has a simple and flexible architecture based on streaming data flows. It is robust and fault tolerant with tunable reliability mechanisms and many failover and recovery mechanisms. It uses a simple extensible data model that allows for online analytic application.
- [Logstash](https://www.elastic.co/products/logstash): Logstash 是一个应用程序日志、事件的传输、处理、管理和搜索的平台。你可以用它来统一对应用程序日志进行收集管理，提供 Web 接口用于查询和统计。
- [FluentD](http://www.fluentd.org/): Fluentd是一个日志收集系统，它的特点在于其各部分均是可定制化的，你可以通过简单的配置，将日志收集到不同的地方。
- [Greylog](https://www.graylog.org/): Free and open source log management
- [Logspout](https://github.com/gliderlabs/logspout): Log routing for Docker container logs
- [Rsyslog](https://github.com/rsyslog/rsyslog): Rsyslog is a rocket-fast system for log processing.
- [Syslog-ng](https://www.syslog-ng.com/)
- [vector](https://vector.dev/): A lightweight and ultra-fast tool for building observability pipelines


## Notebook

- [Jupyter](https://jupyter.org/): The Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, data visualization, machine learning, and much more.
- [PolyNote](https://polynote.org/): The polyglot notebook with first-class Scala support.
