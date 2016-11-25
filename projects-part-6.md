# Projects about Digital Publishing

## Office Document Manipulation

- [NPOI](https://github.com/tonyqus/npoi): NPOI 是 POI 项目的 .NET 版本。POI是一个开源的Java读写Excel、WORD等微软OLE2组件文档的项目。NPOI让.NET平台拥有了一个比较完善的读写Excel的工具。使用量非常广泛，应该是开源的.NET Excel读写工具中曝光度最高的一个吧，没有之一。
- [NPOI扩展—NPOI.CSS](https://github.com/qihangnet/npoi.css): NPOI.CSS是一个可以在使用NPOI时用类CSS的方法设置单元格样式的NPOI扩展，只支持.NET4及以上版本的项目。这个扩展是为了方便在使用的时候设置单元格及其相关格式样式，可以使用类似Css的方式，非常给力。
- [yjinglee.office](https://github.com/YJingLee/yjinglee.office): yjinglee.office用于.Net平台下的Excel操作，主要封装NPOI对外提供更简单实用的API，提供以下功能点：1.读取Excel数据转换成对象集合, 2.写入集合到Excel，并提供可以Excel样式定义
- [Epplus](http://epplus.codeplex.com/): Epplus是一个使用Open Office XML（Xlsx）文件格式，读写Excel 2007/2010文件的开源组件。和NPOI相比，它更早的支持了Xlsx格式，而NPOI支持Excel 2003更好，现在新版本的NPOI也开始支持Xlsx了。支持的范围也很广，例如：单元格合并，单元格样式，图表(这个NPOI目前还不是很好)，表格，数据验证，公式，VBA等等。
- [LinqToExcel](https://github.com/paulyoder/LinqToExcel): LinqToExcel是一个.NET平台下开源项目，它主要实现了LINQ的语法查询Excel电子表格。类型之前的LINQToXXX如果你是LINQ语法糖爱好者那最适合你。
- [NetOffice](http://netoffice.codeplex.com/): NetOffice组件比较特别，是一个操作Office的强大组件，包括处理Office, Excel, Word, Outlook, PowerPoint, Access, Project, Visio等，所以支持非常全面。但是这个组件并不是完全单独写的，而是调用Microsoft Office的互操作程序集以及VSTO，也就是进行了一个深度的封装，从而让你不需要安装这些东西，只需要拷贝相应的程序集就可以了。
- [Word文档读写工具Docx](http://docx.codeplex.com/): DocX is a .NET library that allows developers to manipulate Word 2007/2010/2013 files, in an easy and intuitive manor. DocX is fast, lightweight and best of all it does not require Microsoft Word or Office to be installed.

## PDF Manipulation

- [iText](http://itextpdf.com/product/itext): 打开这个[链接](http://itextpdf.com/functionality)，图里面已经说得很清楚了。
- [PDFSharp](http://www.pdfsharp.net/): PDFsharp is a .NET library for processing PDF file. You create PDF pages using drawing routines known from GDI+. Almost anything that can be done with GDI+ will also work with PDFsharp. Only basic text layout is supported by PDFsharp, and page breaks are not created automatically. The same drawing routines can be used for screen, PDF, or meta files.
- [MigraDoc](http://www.pdfsharp.net/): MigraDoc is a document generator. It supports almost anything you find in any good word processor. You just add paragraphs, tables, charts, arrange all this in sections, use bookmarks to create links, tables of contents, indexes, etc. MigraDoc will do the layout creating page breaks as needed. MigraDoc will create PDF, XPS, or RTF documents.
- [pdftk server](https://www.pdflabs.com/tools/pdftk-server/): PDFtk Server is our command-line tool for working with PDFs. It is commonly used for client-side scripting or server-side processing of PDFs.

## Text Manipulation

- [文件差异比较diffplex](https://github.com/mmanela/diffplex): diffplex是一个开源的C#文本差异比较软件。支持.NET 4.0, Silverlight 5.0, Windows 8.0, Windows Phone 8.0, Windows Phone Appx 8.1等环境。

## OCR

- [tesseract.js](https://github.com/naptha/tesseract.js): Pure Javascript OCR for 62 Languages
- [paperless](https://github.com/danielquinn/paperless): Scan, index, and archive all of your paper documents

## Report

- [ExcelReport报表引擎](https://github.com/hanzhaoxin/ExcelReport): ExcelReport是一款基于NPOI开发的报表引擎组件。它基于关注点分离的理念，将数据与样式、格式分离。让模板承载样式、格式等NPOI不怎么擅长且实现繁琐的信息，结合NPOI对数据的处理的优点将Excel报表的生成化繁为简。同时，对报表组成的基本元素进行了抽象，进一步简化了Excel报表的生成过程。
- [PDFReport](http://pdfreport.codeplex.com/): PdfReport 是一个支持code-first的报表引擎，建立在开源项目iTextSharp和 EPPlus基础上。支持.net 3.5以上
- [ReportGenerator](https://github.com/danielpalme/ReportGenerator): ReportGenerator可以将OpenCover, PartCover, Visual Studio 或者NCover生成的XML报表转换为可读性更加好的格式。上面这几个工具都是代码覆盖率分析工具。转换后的报表有以下格式：1.HTML, HTMLSummary, 2.XML, XMLSummary, 3.Latex, LatexSummary, 4.TextSummary, 5.Custom reports
- [BusyReports - Advanced Report delivery with SQL Server Reporting Services SSRS](http://busyreports.codeplex.com/): BusyReports is an easy to use application to produce reports from the SSRS web services. It is an alternative to the data driven subscriptions of SQL Server.
- [Seal Report](http://sealreport.codeplex.com/): Seal Report offers a complete framework for producing every day reports and dashboards from any database.

## Static Websites Generator

更多参考[StaticGen](https://www.staticgen.com/)

- [Jekyll](http://jekyllrb.com/): Transform your plain text into static websites and blogs.
    - [Jekyllcn](http://jekyllcn.com/)
    - [Octopress](http://octopress.org/)
- [Hexo](https://hexo.io/): A fast, simple & powerful blog framework
