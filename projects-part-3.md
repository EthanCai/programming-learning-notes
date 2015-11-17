# Projects about Data Storage and Analysis

## Database

- [SQL Server](https://msdn.microsoft.com/en-us/library/bb545450.aspx)
- [PostgreSQL](http://www.postgresql.org/):
    - [PostGIS](http://postgis.refractions.net): PostGIS在对象关系型数据库PostgreSQL上增加了存储管理空间数据的能力，相当于Oracle的spatial部分。PostGIS最大的特点是符合并且实现了OpenGIS的一些规范，是最著名的开源GIS数据库。
- [MySQL](http://www.mysql.com/)
- [MariaDB](http://mariadb.org/)
- [WebScaleSQL](http://webscalesql.org/)
- [SQLlite](http://www.sqlite.org/index.html)
- [Apache GEODE](http://geode.incubator.apache.org): Geode is an open source , distributed, in-memory database for scale-out applications.

## Database Engine

- [InnoDB](https://en.wikipedia.org/wiki/InnoDB): InnoDB is a storage engine for MySQL. MySQL 5.5 and later use it by default.[1] It provides the standard ACID-compliant transaction features, along with foreign key support (Declarative Referential Integrity).
- [XtraDB](https://en.wikipedia.org/wiki/XtraDB): Percona XtraDB is a storage engine for the MariaDB and Percona Server databases, and is intended as a drop-in replacement to InnoDB, which is one of the default engines available on the MySQL database.
- [Berkerly DB](http://www.oracle.com/technetwork/database/database-technologies/berkeleydb/overview/index.html): 介绍见[这里](https://en.wikipedia.org/wiki/Berkeley_DB)
- [Tokyo Cabinet](http://fallabs.com/tokyocabinet/): Tokyo Cabinet is a library of routines for managing a database. The database is a simple data file containing records, each is a pair of a key and a value. Every key and value is serial bytes with variable length. Both binary data and character string can be used as a key and a value. There is neither concept of data tables nor data types. Records are organized in hash table, B+ tree, or fixed-length array.
- [Kyoto Cabinet](http://fallabs.com/kyotocabinet/): Kyoto Cabinet is a library of routines for managing a database. The database is a simple data file containing records, each is a pair of a key and a value. Every key and value is serial bytes with variable length. Both binary data and character string can be used as a key and a value. Each key must be unique within a database. There is neither concept of data tables nor data types. Records are organized in hash table or B+ tree.
- [LevelDB](https://github.com/google/leveldb): LevelDB is a fast key-value storage library written at Google that provides an ordered mapping from string keys to string values.
- [tidb](https://github.com/pingcap/tidb): TiDB is a distributed SQL database compatible with MySQL protocol.

## Cache

- [Redis](http://redis.io/): Redis is an open source, BSD licensed, advanced key-value cache and store. It is often referred to as a data structure server since keys can contain strings, hashes, lists, sets, sorted sets, bitmaps and hyperloglogs.
- [Memcached](http://memcached.org/): Free & open source, high-performance, distributed memory object caching system, generic in nature, but intended for use in speeding up dynamic web applications by alleviating database load. Memcached is an in-memory key-value store for small chunks of arbitrary data (strings, objects) from results of database calls, API calls, or page rendering. Memcached is simple yet powerful. Its simple design promotes quick deployment, ease of development, and solves many problems facing large data caches. Its API is available for most popular languages.
- [twemproxy](https://github.com/twitter/twemproxy): A fast, light-weight proxy for memcached and redis
- [shared cache](http://www.sharedcache.com/cms/homepage.aspx): high performance distributed and replication cache system built for .Net applications running in server farms.
- [Infinispan](http://infinispan.org): Infinispan is a distributed in-memory key/value data store with optional schema, available under the Apache License 2.0. It can be used both as an embedded Java library and as a language-independent service accessed remotely over a variety of protocols (HotRod, REST, Memcached and WebSockets). It offers advanced functionality such as transactions, events, querying and distributed processing.
- [Apache Ignite](https://ignite.incubator.apache.org/): Apache Ignite In-Memory Data Fabric is a high-performance, integrated and distributed in-memory platform for computing and transacting on large-scale data sets in real-time, orders of magnitude faster than possible with traditional disk-based or flash technologies.

## NoSQL Database

- [MongoDB](https://www.mongodb.org/)
- [TokuMX](http://www.tokutek.com/): High-Performance MongoDB
- [InfluxDB](https://influxdb.com/index.html): An open-source distributed time series database with no external dependencies.
- [RavenDB](http://ravendb.net/): A linq enabled document database for .NET
- [EventStore](https://github.com/EventStore/EventStore): The open-source, functional database with Complex Event Processing in JavaScript.
- [LevelDB](https://github.com/google/leveldb): LevelDB is a fast key-value storage library written at Google that provides an ordered mapping from string keys to string values.
    - [eLevelDB](https://github.com/basho/eleveldb): eLevelDB 是一个 Erlang 应用程序，封装了 LevelDB
- [Cassandra](http://cassandra.apache.org/): The Apache Cassandra database is the right choice when you need scalability and high availability without compromising performance. Linear scalability and proven fault-tolerance on commodity hardware or cloud infrastructure make it the perfect platform for mission-critical data. Cassandra's support for replicating across multiple datacenters is best-in-class, providing lower latency for your users and the peace of mind of knowing that you can survive regional outages.

## Data Warehouse

- [infobright community edition](https://www.infobright.com/)
- [Greenplum Database](http://greenplum.org): Greenplum DB 号称是世界上第一个开源的大规模并行数据仓库，最初是基于 PostgreSQL，现在已经添加了大量数据库方面的创新。Greenplum 提供 PD 级别数据量的强大和快速分析能力，特别是面向大数据方面的分析能力，支持大数据的超高性能分析查询。

## Search

- [Apache Solr](http://lucene.apache.org/solr/): Solr is the popular, blazing-fast, open source enterprise search platform built on Apache Lucene.
    - [mmseg4j-solr](https://github.com/chenlb/mmseg4j-solr): mmseg4j for lucene or solr analyzer
    - [mmseg4j-core](https://github.com/chenlb/mmseg4j-core): mmseg4j core MMSEG for java chinese analyzer
- [ElasticSearch](https://www.elastic.co/): elasticsearch 的目标是解决上面的所有问题以及更多。她是开源的（Apache2协议），分布式的，RESTful的，构建在Apache Lucene之上的的搜索引擎.
    - [elasticsearch-rtf](https://github.com/medcl/elasticsearch-rtf): elasticsearch中文发行版，针对中文集成了相关插件，并带有Demo，方便新手学习,或者在生产环境中直接使用
    - [elasticsearch-analysis-ik](https://github.com/medcl/elasticsearch-analysis-ik): The IK Analysis plugin integrates Lucene IK analyzer into elasticsearch, support customized dictionary.
    - [elasticsearch-analysis-mmseg](https://github.com/medcl/elasticsearch-analysis-mmseg): Mmseg Analysis for ElasticSearch
    - [elasticsearch-analysis-pinyin](https://github.com/medcl/elasticsearch-analysis-pinyin): The Pinyin Analysis plugin integrates Pinyin4j(http://pinyin4j.sourceforge.net/) module into elasticsearch.
- [Sphinx](http://sphinxsearch.com/): Sphinx Search 是由俄罗斯人Andrew Aksyonoff 开发的高性能全文搜索软件包，在GPL与商业协议双许可协议下发行。Sphinx is an open source full text search server, designed from the ground up with performance, relevance (aka search quality), and integration simplicity in mind. It's written in C++ and works on Linux (RedHat, Ubuntu, etc), Windows, MacOS, Solaris, FreeBSD, and a few other systems.
    - [sphinx-for-chinese](http://sphinx-search.com/): sphinx-for-chinese是一款专注于中文搜索的全文检索软件，在sphinx的基础上添加了中文处理模块并优化了中文搜索效果。
- [xunsearch](http://www.xunsearch.com/): 开源免费、高性能、多功能, 简单易用的专业全文检索技术方案
- [bleve](https://github.com/blevesearch/bleve): A modern text indexing library for go
- [Apache Nutch](http://nutch.apache.org/): Apache Nutch是一个用Java编写的开源网络爬虫。Apache Nutch对于Solr已经支持得很好，这大大简化了Nutch与Solr的整合。
- [Apache Tika](http://tika.apache.org/): The Apache Tika™ toolkit detects and extracts metadata and text from over a thousand different file types (such as PPT, XLS, and PDF). All of these file types can be parsed through a single interface, making Tika useful for search engine indexing, content analysis, translation, and much more.

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
- [basho](http://basho.com/): Introducing the Basho Data Platform. The most powerful way to manage today’s active workloads for Big Data.
- [Apache Spark](http://spark.apache.org/): a fast and general engine for large-scale data processing
- [Apache TAJO](http://tajo.apache.org/): A big data warehouse system on Hadoop
- [Apache Kylin](http://kylin.incubator.apache.org/): Apache Kylin is an open source Distributed Analytics Engine from eBay Inc. that provides SQL interface and multi-dimensional analysis (OLAP) on Hadoop supporting extremely large datasets
- [Apache Hive](http://hive.apache.org/): The Apache Hive ™ data warehouse software facilitates querying and managing large datasets residing in distributed storage. Hive provides a mechanism to project structure onto this data and query the data using a SQL-like language called HiveQL. At the same time this language also allows traditional map/reduce programmers to plug in their custom mappers and reducers when it is inconvenient or inefficient to express this logic in HiveQL.
- [Apache HBase](http://hbase.apache.org/): Apache HBase™ is the Hadoop database, a distributed, scalable, big data store
- [Apache HAWQ](http://hawq.incubator.apache.org): HAWQ 是 Pivotal 设计的一个大规模并行 SQL 分析处理引擎，支持事务处理。HAWQ 将复杂的查询分割成简单的任何，并分发到并行处理系统中的处理单元执行。包括查询规划器、动态管道、前沿互联和查询执行优化器等等。提供最高级别的性能和可伸缩性。HAWQ 基于 Hadoop 架构。

## Distributed realtime computation system

- [Apache Storm](http://storm.apache.org/): Storm has many use cases: realtime analytics, online machine learning, continuous computation, distributed RPC, ETL, and more. Storm is fast: a benchmark clocked it at over a million tuples processed per second per node. It is scalable, fault-tolerant, guarantees your data will be processed, and is easy to set up and operate.
- [jstorm](https://github.com/alibaba/jstorm): JStorm is a distributed and fault-tolerant realtime computation system. Inspired by Apache Storm, JStorm has been completely rewritten in Java and provides many more enhanced features. JStorm has been widely used in many enterprise environments and proved robust and stable.
- [Twitter Heron](http://dl.acm.org/citation.cfm?id=2742788): 参考[Twitter发布新的大数据实时分析系统Heron](http://geek.csdn.net/news/detail/33750)
- [Apache Samza](http://samza.apache.org/): Apache Samza is a distributed stream processing framework. It uses Apache Kafka for messaging, and Apache Hadoop YARN to provide fault tolerance, processor isolation, security, and resource management.
- [Apache Kafka](http://kafka.apache.org/): Apache Kafka is publish-subscribe messaging rethought as a distributed commit log.
- [Apache Flink](http://flink.apache.org/): Apache Flink is an open source platform for scalable batch and stream data processing.

## Data Visualization

- [nflabs](http://www.nflabs.com/): Introducing a new way to do big data analysis, Visualize, analyze, and collaborate on big data without the hassle of big data
    - [Apache Zeppelin](https://zeppelin.incubator.apache.org/): A web-based notebook that enables interactive data analytics. You can make beautiful data-driven, interactive and collaborative documents with SQL, Scala and more.
- [kibana](https://www.elastic.co/products/kibana): Kibana 是一个为 Logstash 和 ElasticSearch 提供的日志分析的 Web 接口。可使用它对日志进行高效的搜索、可视化、分析等各种操作。
- [Grafana](http://grafana.org/): Grafana is a leading open source application for visualizing large-scale measurement data.

## Machine Learning and Data Science

- [Accord.NET](http://accord-framework.net/) - Machine learning framework combined with audio and image processing libraries (computer vision, computer audition, signal processing and statistics).
- [Accord.NET Extensions](https://github.com/dajuric/accord-net-extensions) - Advanced image processing and computer vision algorithms made as fluent extensions.
- [AForge.NET](http://www.aforgenet.com/) - Framework for developers and researchers in the fields of Computer Vision and Artificial Intelligence (image processing, neural networks, genetic algorithms, machine learning, robotics).
- [PredictionIO](https://prediction.io/): An open-source machine learning server for developers and data scientists to create predictive engines for production environments, with zero downtime training and deployment.
- [Apache Mahout](https://mahout.apache.org/): The Apache Mahout™ project's goal is to build an environment for quickly creating scalable performant machine learning applications.
- [Aerosolve - Airbnb](http://airbnb.io/aerosolve/): A machine learning package built for humans.
- [Caffe](http://caffe.berkeleyvision.org/): Caffe is a deep learning framework made with expression, speed, and modularity in mind. It is developed by the Berkeley Vision and Learning Center (BVLC) and by community contributors. Yangqing Jia created the project during his PhD at UC Berkeley. Caffe is released under the BSD 2-Clause license.
- [golearn](https://github.com/sjwhitworth/golearn): Machine Learning for Go
- [shogun](https://github.com/shogun-toolbox/shogun): The Shogun Machine learning toolbox provides a wide range of unified and efficient Machine Learning (ML) methods. The toolbox seamlessly allows to easily combine multiple data representations, algorithm classes, and general purpose tools. This enables both rapid prototyping of data pipelines and extensibility in terms of new algorithms. We combine modern software architecture in C++ with both efficient low-level computing backends and cutting edge algorithm implementations to solve large-scale Machine Learning problems (yet) on single machines.

## Log Process

- [Apache Flume](http://flume.apache.org/): Flume is a distributed, reliable, and available service for efficiently collecting, aggregating, and moving large amounts of log data. It has a simple and flexible architecture based on streaming data flows. It is robust and fault tolerant with tunable reliability mechanisms and many failover and recovery mechanisms. It uses a simple extensible data model that allows for online analytic application.
- [Logstash](https://www.elastic.co/products/logstash): Logstash 是一个应用程序日志、事件的传输、处理、管理和搜索的平台。你可以用它来统一对应用程序日志进行收集管理，提供 Web 接口用于查询和统计。
- [FluentD](http://www.fluentd.org/): Fluentd是一个日志收集系统，它的特点在于其各部分均是可定制化的，你可以通过简单的配置，将日志收集到不同的地方。
