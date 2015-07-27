# 说明

这是一本手册，帮助你使用（但不仅限于）dotNET开发更好的应用。

备注：

- [website-attack-and-defense.md](./website-attack-and-defense.md): 常见的网络攻击手段和防御方法
- [magic-fsharp](./magic-fsharp/md): F#学习资料

-------------------------------------------------------------------------------

# Books

- [CLR via C#](http://book.douban.com/subject/4924165/)
- [C# in Depth](http://book.douban.com/subject/3133747/) - [图书官网](http://csharpindepth.com/)
- [Threading in C#](http://www.albahari.com/threading/)
- [Concurrency in C# Cookbook](http://book.douban.com/subject/25899958/)
- [Windows并发编程指南](http://book.douban.com/subject/4214617/)
- [Pro .NET Best Practices](http://www.amazon.com/NET-Best-Practices-Experts-Voice/dp/1430240237/ref=sr_1_1)
- [Pro C# 5.0 and the .NET 4.5 Framework, 6th Edition](http://www.amazon.com/Pro-NET-Framework-Experts-Voice/dp/1430242337/ref=sr_1_1)

-------------------------------------------------------------------------------

# Code Style Guide

- [NET设计规范：约定、惯用法与模式](http://book.douban.com/subject/4231292/)
- [C# 3.0, C# 4.0 and C# 5.0 Coding Guidelines](http://csharpguidelines.codeplex.com/)
- [Style guides for Google-originated open-source projects](https://github.com/google/styleguide)
- [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)

-------------------------------------------------------------------------------

# Foundation, Organization, Specification

## Organization

- [.NET Foundation](http://www.dotnetfoundation.org)
- [patterns & practices](https://msdn.microsoft.com/en-us/library/ff921345.aspx)
- [ServiceStack](https://servicestack.net/)
- [StackExchange](https://github.com/StackExchange)
- [Castle Projects](http://www.castleproject.org)
- [Mono Projects](https://github.com/mono)

## Specification

- [OWIN - Open Web Interface for .NET](http://owin.org/)
- [OData](http://odata.github.io/): OData is an OASIS standard for creating and consuming RESTful APIs.
- HTTP
    - [HTTP/2 Protocol](http://http2.github.io/): HTTP/2 is a replacement for how HTTP is expressed “on the wire.” It is not a ground-up rewrite of the protocol; HTTP methods, status codes and semantics are the same, and it should be possible to use the same APIs as HTTP/1.x (possibly with some small additions) to represent the protocol.
    - [HTTP/2 explained](http://daniel.haxx.se/http2/): http2 explained describes the protocol HTTP/2 at a technical and protocol level. Background, the protocol, the implementations and the future. Written by Daniel Stenberg.
- Data Exchange Format
    - [Portocol Buffer](https://developers.google.com/protocol-buffers/): Protocol buffers are Google's language-neutral, platform-neutral, extensible mechanism for serializing structured data – think XML, but smaller, faster, and simpler. 
    - [Message Pack](http://msgpack.org/): MessagePack is an efficient binary serialization format. It lets you exchange data among multiple languages like JSON. But it's faster and smaller. Small integers are encoded into a single byte, and typical short strings require only one extra byte in addition to the strings themselves.
    - [Apache Thrift](http://thrift.apache.org/): Thrift源于大名鼎鼎的facebook之手，在2007年facebook提交Apache基金会将Thrift作为一个开源项目，对于当时的facebook来说创造thrift是为了解决facebook系统中各系统间大数据量的传输通信以及系统之间语言环境不同需要跨平台的特性。所以thrift可以支持多种程序语言，例如: C++, C#, Cocoa, Erlang Haskell, Java, Ocami, Perl, PHP, Python, Ruby, Smalltalk. 在多种不同的语言之间通信thrift可以作为二进制的高性能的通讯中间件，支持数据(对象)序列化和多种类型的RPC服务。Thrift适用于程序对程序静态的数据交换，需要先确定好他的数据结构，他是完全静态化的，当数据结构发生变化时，必须重新编辑IDL文件，代码生成，再编译载入的流程，跟其他IDL工具相比较可以视为是Thrift的弱项，Thrift适用于搭建大型数据交换及存储的通用工具，对于大型系统中的内部数据传输相对于JSON和xml无论在性能、传输大小上有明显的优势。
    - [Apache Avro](http://avro.apache.org/): Apache Avro™ is a data serialization system.
    - [Cap’n Proto](https://capnproto.org/index.html): Cap’n Proto is an insanely fast data interchange format and capability-based RPC system. Think JSON, except binary. Or think Protocol Buffers, except faster. In fact, in benchmarks, Cap’n Proto is INFINITY TIMES faster than Protocol Buffers.
    - [Microsoft bond](https://github.com/Microsoft/bond): Bond is a cross-platform framework for working with schematized data. It supports cross-language de/serialization and powerful generic mechanisms for efficiently manipulating data. Bond is broadly used at Microsoft in high scale services.
    - [JSON](http://json.org/): JSON (JavaScript Object Notation) is a lightweight data-interchange format. It is easy for humans to read and write. It is easy for machines to parse and generate. It is based on a subset of the JavaScript Programming Language, Standard ECMA-262 3rd Edition - December 1999. JSON is a text format that is completely language independent but uses conventions that are familiar to programmers of the C-family of languages, including C, C++, C#, Java, JavaScript, Perl, Python, and many others. These properties make JSON an ideal data-interchange language.
        - [JSON Schema](http://json-schema.org/)
        - [JSON Schema Generator](http://jsonschema.net/)

-------------------------------------------------------------------------------

# Projects

- [.NET Framework & Libs](./projects-part-1.md)
- [Distributed Architecture](./projects-part-2.md)
- [Data Storage and Analysis](./projects-part-3.md)
- [DevOps](./projects-part-4.md)

# Articles

- [.NET Language & CLR](./articles-part-1.md)
- [Distributed Architecture](./articles-part-2.md)
- [Data Storage and Analysis](./articles-part-3.md)
- [DevOps](./articles-part-4.md)

-------------------------------------------------------------------------------

# References

- [official home of .NET on GitHub](https://github.com/microsoft/dotnet): dotnet is the official home of .NET on GitHub. It's a great starting point to find many .NET OSS projects from Microsoft and the community, including many that are part of the .NET Foundation.
- [Patterns & Practices](https://msdn.microsoft.com/en-us/library/ff921345.aspx)
- [Awesome dotNET](https://github.com/quozd/awesome-dotnet)
- [Open Source Testing](http://www.opensourcetesting.org/)
- [NoSQL Database](http://nosql-database.org/)
- [amplab - UC BERKELEY](https://amplab.cs.berkeley.edu/)
- [A Complete List of .NET Open Source Developer Projects](http://scottge.net/2015/07/08/a-complete-list-of-net-open-source-developer-projects/)