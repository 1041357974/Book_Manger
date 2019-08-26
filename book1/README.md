# Book_Manger
图书管理系统
xml-使用dom4j对xml文件进行crud操作
一、简介。

1.xml解析技术有两种：dom和sax

2.dom:Document Object Model,即文档对象模型，是W3C组织推荐的解析XML的一种方式。

sax:Simple API for XML，不是官方标准，单它是xml社区事实上的标准。

3.XML解析器：Crimson(sun,jdk自带)、Xerces(IBM 最好的解析器)、A elfred2(dom4j)，使用哪种解析器对程序员基本上没有什么影响，我们学习的是解析开发包，解析开发包调用什么样的解析器对程序员没有意义。

4.XML解析开发包：Jaxp(sun)、Jdom（不推荐使用）、dom4j(比较不错)，Pull（android的sdk自带,它使用的是另外的解析方式streaming api for xml,即stax）

5.JAXP：Java API for xml Processing,jaxp是sun提供的一套xml解析API,jaxp很好地支持了dom和sax解析方式

解析XML文档使用的包名：

javax.xml
org.xml.sax
org.w3c.dom

javax.xml.parsers包中，定义了几个工厂类，程序员调用这些工程类，可以得到对xml文档进行解析的dom或者sax的解析器对 
象。

6.DOM解析过程：首先将整个文档加载到内存，形成DOM树。使用dom进行解析，得到Document对象

7.使用DOM解析方式的缺点：整个文档需要全部放入内存，如果是大文件极易出现内存溢出的情况。

使用DOM解析方式的有点：操作速度快。
