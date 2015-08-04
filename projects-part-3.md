# Projects about Data Storage and Analysis

## Database

- [SQL Server](https://msdn.microsoft.com/en-us/library/bb545450.aspx)
- [PostgreSQL](http://www.postgresql.org/)
- [MySQL](http://www.mysql.com/)
- [MariaDB](http://mariadb.org/)
- [WebScaleSQL](http://webscalesql.org/)
- [SQLlite](http://www.sqlite.org/index.html)

## Cache

- [Redis](http://redis.io/): Redis is an open source, BSD licensed, advanced key-value cache and store. It is often referred to as a data structure server since keys can contain strings, hashes, lists, sets, sorted sets, bitmaps and hyperloglogs.
- [Memcached](http://memcached.org/): Free & open source, high-performance, distributed memory object caching system, generic in nature, but intended for use in speeding up dynamic web applications by alleviating database load. Memcached is an in-memory key-value store for small chunks of arbitrary data (strings, objects) from results of database calls, API calls, or page rendering. Memcached is simple yet powerful. Its simple design promotes quick deployment, ease of development, and solves many problems facing large data caches. Its API is available for most popular languages.
- [twemproxy](https://github.com/twitter/twemproxy): A fast, light-weight proxy for memcached and redis
- [shared cache](http://www.sharedcache.com/cms/homepage.aspx): high performance distributed and replication cache system built for .Net applications running in server farms.

## NoSQL Database

- [MongoDB](https://www.mongodb.org/)
- [TokuMX](http://www.tokutek.com/): High-Performance MongoDB
- [InfluxDB](https://influxdb.com/index.html): An open-source distributed time series database with no external dependencies.
- [RavenDB](http://ravendb.net/): A linq enabled document database for .NET

## Data Analytics

- [infobright community edition](https://www.infobright.com/)

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