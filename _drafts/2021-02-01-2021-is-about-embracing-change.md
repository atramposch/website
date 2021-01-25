---
 layout: post
 title: "Data Transfer using XML or JSON"
 author: Andrew Tramposch
 date: 2021-02-01
 date_2: 2021-02-01
 new_expire_date: 2021-02-15
---
Moving data from one place to another is one of the most important functions in today's ever connected society. For years, programmers used simple text files or comma separated values to translate data from one program or computer to another. These were not necessarily "human-readable" and if they were provided in binary format, you'd need a specific program to view or edit. How do we translate data in a structured format that is "human-readable" and potentially self-validating? 

## Here comes XML, a brief history
In 1970 Charles Goldfarb, Ed Mosher & Ray Lorie invented GML, a way of marking up technical documents with structural tags. GML stood for their initials but they soon coined the term "mark-up language" and GML soon became Standard Generalized Markup Language (SGML). This naming is a little confusing as SGML is not actually itself a markup language, but rather a specification adopted by ISO in 1986. This specification soon birthed the ever important HTML (Hypertext Markup Language). HTML applies the specifications set forth by SGML and defines a specific set of tags that can be used in the creation of web pages. HTML was quickly adopted as the advent of the internet loomed. 

The original thinking for HTML, and web pages in general, was to separate content from presentation. This means that all tags created in an HTML file were left up to browsers to interpret, and no two browsers interpreted in the same way. This type of issue did not please web designers who wanted to ensure their pages displayed as designed. The competition between browsers at the time led to further fragmentation of the HTML standard, which still remains an issue for web developers today. 

With the issues and limitations observed by HTML and the complexity of SGML daunting, XML, eXtensible Markup Language, was born. Like SGML, XML itself is not a language and in fact just a standard specification for defining markup languages. XML can be described as a 'meta markup language' and its purpose was to simplify SGML by focusing on a particular problem - documents on the internet. 'Meta markup language' allows users to create any tags needed (hence 'eXtensible') and then describing those tags and their permitted uses. 

You might have seen plenty of 'save as .xml' options in Microsoft products or other applications. The simple fact of a document being saved in XML format does not guarantee any usefulness or ability to transfer data between applications. For example, you might save a file in XML format from Microsoft Word. These are large documents with hundreds of Microsoft Word specific elements and attributes. Just because it is XML does not mean that Apple  or Illustrator can open this file, read the contents, and let you begin editing in a native file format. It might be possible for the developer of that software to create an import tool for that specific XML format from that specific application, but without that added functionality there is no "out of the box" interoperability. It would take all drawing application developers  
