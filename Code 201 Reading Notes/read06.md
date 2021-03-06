 # **Introduction to the DOM**
- The Document Object Model (DOM) is the data representation of the objects that comprise the structure and content of a document on the web. In this guide, we'll briefly introduce the DOM. We'll look at how the DOM represents an HTML or XML document in memory and how you use APIs to create web content and applications.
### What is the DOM?
The Document Object Model (DOM) is a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page.
A Web page is a document. This document can be either displayed in the browser window or as the HTML source. But it is the same document in both cases. The Document Object Model (DOM) represents that same document so it can be manipulated. The DOM is an object-oriented representation of the web page, which can be modified with a scripting language such as JavaScript.
The W3C DOM and WHATWG DOM standards are implemented in most modern browsers. Many browsers extend the standard, so care must be exercised when using them on the web where documents may be accessed by various browsers with different DOMs.
For example, the standard DOM specifies that the querySelectorAll method in the code below must return a list of all the <p> elements in the document:
const paragraphs = document.querySelectorAll("p");
// paragraphs[0] is the first <p> element
// paragraphs[1] is the second <p> element, etc.
alert(paragraphs[0].nodeName);
developer.mozilla.orgdeveloper.mozilla.org
HTML - MDN Web Docs Glossary: Definitions of Web-related terms | MDN
HTML (HyperText Markup Language) is a descriptive language that specifies webpage structure.
developer.mozilla.orgdeveloper.mozilla.org
XML - MDN Web Docs Glossary: Definitions of Web-related terms | MDN
eXtensible Markup Language (XML) is a generic markup language specified by the W3C. The information technology (IT) industry uses many languages based on XML as data-description languages.
developer.mozilla.orgdeveloper.mozilla.org
Introduction to the DOM - Web APIs | MDN
The Document Object Model (DOM) is the data representation of the objects that comprise the structure and content of a document on the web. In this guide, we'll briefly introduce the DOM.





20:59
All of the properties, methods, and events available for manipulating and creating web pages are organized into objects (for example, the document object that represents the document itself, the table object that implements the special HTMLTableElement DOM interface for accessing HTML tables, and so forth). This documentation provides an object-by-object reference to the DOM.
The modern DOM is built using multiple APIs that work together. The core DOM defines the objects that fundamentally describe a document and the objects within it. This is expanded upon as needed by other APIs that add new features and capabilities to the DOM. For example, the HTML DOM API adds support for representing HTML documents to the core DOM.
DOM and JavaScript
The short example above, like nearly all of the examples in this reference, is JavaScript. That is to say, it's written in JavaScript, but it uses the DOM to access the document and its elements. The DOM is not a programming language, but without it, the JavaScript language wouldn't have any model or notion of web pages, HTML documents, XML documents, and their component parts (e.g. elements). Every element in a document—the document as a whole, the head, tables within the document, table headers, text within the table cells—is part of the document object model for that document, so they can all be accessed and manipulated using the DOM and a scripting language like JavaScript.
In the beginning, JavaScript and the DOM were tightly intertwined, but eventually, they evolved into separate entities. The page content is stored in the DOM and may be accessed and manipulated via JavaScript, so that we may write this approximative equation:
API = DOM + JavaScript
The DOM was designed to be independent of any particular programming language, making the structural representation of the document available from a single, consistent API. Though we focus exclusively on JavaScript in this reference documentation, implementations of the DOM can be built for any language, as this Python example demonstrates:
# Python DOM example
import xml.dom.minidom as m
doc = m.parse(r"C:\Projects\Py\chap1.xml")
doc.nodeName # DOM property of document object
p_list = doc.getElementsByTagName("para")
For more information on what technologies are involved in writing JavaScript on the web, see JavaScript technologies overview.
Accessing the DOM
You don't have to do anything special to begin using the DOM. Different browsers have different implementations of the DOM, and these implementations exhibit varying degrees of conformance to the actual DOM standard (a subject we try to avoid in this documentation), but every web browser uses some document object model to make web pages accessible via JavaScript.
When you create a script–whether it's inline in a  element or included in the web page by means of a script loading instruction–you can immediately begin using the API for the document or window elements to manipulate the document itself or to get at the children of that document, which are the various elements in the web page. Your DOM programming may be something as simple as the following, which displays an alert message by using the alert() function from the window object, or it may use more sophisticated DOM methods to actually create new content, as in the longer example below.
This following JavaScript will display an alert when the document is loaded (and when the whole DOM is available for use):
20:59
 onload="window.alert('Welcome to my home page!')
Another example. This function creates a new H1 element, adds text to that element, and then adds the H1 to the tree for this document