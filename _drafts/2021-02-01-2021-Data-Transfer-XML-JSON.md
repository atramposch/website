---
 layout: post
 title: "Data Transfer using XML or JSON"
 author: Andrew Tramposch
 tag: Software
 date: 2021-02-01
 date_2: 2021-02-01
 new_expire_date: 2021-02-15
---
Moving data from one place to another is one of the most important functions in today's ever connected society. For years, programmers used simple text files or comma separated values to translate data from one program or computer to another. These were not necessarily "human-readable" and if they were provided in binary format, you'd need a specific program to view or edit. How do we translate data in a structured format that is "human-readable" and potentially self-validating? 

## Here comes XML, a brief history
In 1970 Charles Goldfarb, Ed Mosher & Ray Lorie invented GML, a way of marking up documents with "structural tags". These tags helped enhance text editing with formatting, and allow for information retrieval systems to work well with the documents they created. GML stood for their initials but they soon coined the term "mark-up language" and GML soon became Standard Generalized Markup Language (SGML) adopted by ISO and ANSI standards in 1986. One item to note is that SGML is not a markup language, but a way of defining a markup language. 

At about the same time as SGML came HTML. The purpose of HTML, and the World Wide Web was so employees across the globe could share and update information for each other to see. Originally developed solely for a singular platform, the creator Tim Berners-Lee put the specifications and code for the entire HTML project on the internet, sparking interest throughout the internet community. HTML was quickly adopted as the advent of the internet loomed. As web grew more and more, more online documents were being produced, and various implementations of HTML grew, but no standardized set of HTML tags appeared. 

HTML evolved to become only useful for presentation layers and not data descriptions, transfers, or anything inbetween. It was believed that HTML was limite and due to the overarching complexity of SGML, XML, eXtensible Markup Language, was born. XML can be described as a 'meta markup language' and its purpose was to simplify SGML by focusing on a particular problem - documents on the internet. 'Meta markup language' allows users to create any tags needed (hence 'eXtensible') and then describe those tags and their permitted uses. It is a simple text-based format for representing structured information: documents, data, configuration, books, transactions, and much more. The best part was it was easily readable by both machines and humans. Once again it is important to note that XML is not a markup language, but in fact a way of defining a markup language. Ultimately, XML was created as a means to provide a data vocabulary. This enabled the data to come with context instead of just data alone. 

Let's give an example of what XML is not. You might have seen plenty of 'save as .xml' options in Microsoft products or other applications. The simple fact of a document being saved in XML format does not guarantee any usefulness or ability to transfer data between applications. For example, you might save a file in XML format from Microsoft Word. These could be large documents with hundreds of Microsoft Word specific elements and attributes. Just because it is XML does not mean that Apple Pages or Adobe Illustrator can open this file, read the contents, and let you begin editing in a native file format. It might be possible for the developer of that software to create an import tool for that specific XML format from that specific application, but without that added functionality there is no "out of the box" interoperability. This is where standardization comes into play and different entities must collaborate. 

## XML Structure 

Typical XML Syntax:
~~~xml
<?xml Definition>
<root>
    <child>
        <subchild>.....</subchild>
    <child>
</root>
~~~
### XML Definition
~~~xml
<?xml version="1.0" encoding="UTF-8"?>
~~~
This is an optional field but usage is typical and its use is incredibly important to define the the metadata intended to be used in the XML file below this point. It contains the XML version attribute and the XML file encoding attribute. There is no closing tag required. 

The version attribute ironically has no other options than "1.0". For the encoding attribute it will be important to select the encoding that encompasses the character set you intend to use. For example, if you live in the US, ASCII could work, but in many other countries characters like ä, å, ü etc. are needed. You'd get some weird characters if you set the encoding to ASCII and needed those characters. There are various different types of file encoding, example: UTF-8 (most commonly used), UTF-16, UTF-32, ISO-8859 and plenty of other options. 

## Root Element
~~~xml
<?xml version="1.0" encoding="UTF-8"?>
<school>
    <name>PS 101</name>
    <district>12</district>
</school>
~~~
This is a mandatory field and is the parent of all the elements. All of the other elements to be defined in XML should and must be inside one root element. There can only be one root element in the XML file. 

Citations

1. Quin, L. XML Essentials. W3C. 1/26/2021, from https://www.w3.org/standards/xml/core
2. Szul, M. (February 15th, 2015). A Brief History of Markup & XML. Codepunk. 1/26/2021, from https://codepunk.io/a-brief-history-of-markup-and-xml/ 