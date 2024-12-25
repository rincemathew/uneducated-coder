# HTML

## HTML BASICS

### HTML
HTML stands for HyperText Markup Language. It is used to design web pages using a markup language. HTML is a combination of Hypertext and Markup language. Hypertext(Hypertext is text which contains links to other texts) defines the link between the web pages. The markup language is used to define the text document within the tag which defines the structure of web pages. HTML is used to structure the website and is therefore used for Web Development.
https://html.spec.whatwg.org/
https://en.wikipedia.org/wiki/Hypertext
https://www.geeksforgeeks.org/what-is-hypertext/

### Markup language
A markup language is a set of rules(no logic in markup languages) governing what markup information may be included in a document and how it is combined with the content of the document in a way to facilitates use by humans and computer programs.
A markup tag is a directive that contains snippet of code with a relative reference to an object in your store such as a variable, URL, image, or block.
Eg:html, xml etc

### What is <!DOCTYPE html>?
<!DOCTYPE html> is a document type declaration (DOCTYPE) used in HTML to specify the version of HTML the document is written in. It is not a tag but an instruction to the web browser about what version of HTML the page is using.
In modern web development, <!DOCTYPE html> is the declaration for HTML5.

### <html> tag?
The <html> tag is the root element of an HTML document. It represents the entire HTML structure and contains all the content of the web page, including metadata and visible content.
other words
The <html> tag defines the starting point of the HTML document, letting browsers understand how to process and render the content inside it.

#### <html> attributes
**lang**: Specifies the language of the document's content (e.g., lang="en" for English).
##### Why Use lang Attribute?
*Accessibility*: Screen readers and other assistive technologies use the lang attribute to read text in the correct language.
*Search Engine Optimization (SEO)*: Search engines like Google may use the language attribute to provide more relevant search results to users.
*Localization*: Browsers and translation tools use this attribute to understand the primary language of the page.
Common Language Codes:
The value of lang is based on the ISO 639-1 standard. Examples include:en: English, es: Spanish, fr: French, de: German, zh: Chinese, ar: Arabic
**dir**: Defines the text direction (ltr for left-to-right, rtl for right-to-left languages like Arabic or Hebrew).

### <meta> tag?
The <meta> tag in HTML provides metadata about the web page. Metadata is information that helps browsers and search engines understand the content and behavior of the web page. The <meta> tag is always placed inside the <head> section and does not have a closing tag.
Why Are <meta> Tags Important?
Improved SEO: Help search engines understand your content better.
Enhanced User Experience: Ensure pages are mobile-friendly and load properly.
Social Media Sharing: Control how your page looks when shared on platforms like Facebook or Twitter.
Accessibility: Specify important information for browsers and assistive technologies.

eg:<meta http-equiv="refresh" content="3; url=https://example.com">
this use for Automatically refreshes or redirects the page after a specified time.

#### What is <meta name="viewport" content="width=device-width, initial-scale=1.0">?
The <meta name="viewport" content="width=device-width, initial-scale=1.0"> tag is a crucial element for building responsive web pages that adapt well to different screen sizes, especially on mobile devices.
**name="viewport"**:Specifies that this meta tag is for controlling the viewport, which is the user's visible area of a web page.
**content="width=device-width"**:Sets the width of the viewport to be the same as the device's screen width. Ensures the content fits the screen size without unnecessary horizontal scrolling.
**initial-scale=1.0"**:Sets the initial zoom level of the page. 1.0 means no zoom (the page appears at its actual size).

#### <meta charset="UTF-8">?
UTF-8 (Unicode Transformation Format-8-bit) is a character encoding standard that represents characters using one to four bytes.
Character encoding is the process of assigning numbers to characters, such as letters, numbers, and symbols, so that computers can interpret them. This allows computers to store, transmit, and transform these characters.
https://www.w3schools.com/charsets/ref_html_utf8.asp
https://naveenr.net/unicode-character-set-and-utf-8-utf-16-utf-32-encoding/

### custom data attribute?
It is part of the HTML5 data- attribute standard*, which allows developers to store custom data in HTML elements. These attributes are primarily used for embedding additional information that can be accessed via JavaScript.
eg: <div class="cell" data-cell></div>

#### async and defer
Scripts loaded with the defer attribute will load in the order they appear on the page. They won't run until the page content has all loaded
eg: <script src="script.js" defer></script>
https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script

## HTML INDEPTH

## HTML EXTRAS


Text document

Html vs html5
html5 is a buzzword to refer to modern web technologies

Trees
doubly liked list - node
benifites = traversal and search

Html element and tag
HTML Block and Inline Elements
Semantic elements 
Technically, an HTML element is the collection of start tag, its attributes, an end tag and everything in between. On the other hand an HTML tag (either opening or closing) is used to mark the start or end of an element, as you can see in the above illustration.


html tags

Html attributes 
Dfdf

html elements


kind of content
https://html.spec.whatwg.org/multipage/dom.html#metadata-content-2

Html headings
Dfdf


Html paragraph
Dsfdf

HTML Entities

Difference between html vs xhtml

the document
doucment types

html is the root of html document

metadata, character set


container body,header,footer etc

////
ASCII-based plain text are being replaced with Unicode as a universal character encoding.
<div> = division
<b> vs <strong>
<em> vs <i>

#### group things
quotes
unordered list
ordered list
association list dl, dt, dd


<em>, <strong>, <small>, <br>

<!--- --->

<span>

http

hypertext - text that references other text which the user agent enables the user to immediately access.

protocol - a system of rules for two entities to communicate.

server - a computer or software that manages access to services and resources( like documents, images, and video)

hypertext transfer protocol - a set of rules for how two entities (client and server) can transfer text between themselves. Text which can link user to other related text.

anchor tags, Hyperlinks, href

rendering engine
a computer program that trasnforms an html dicumet into a visual, interactive repersentation of the dicument for the user.
eg: blink (chromium rendering engine), gecko(mozilla), webkit(safari)

parse

names character reference
&lt; for >

objects 
A collection of data (information) and code (that accomplishes things) which together repersents something.

Document object model
an object model that repersents an html document, providing the abliity to examine and change the document as presented via the user agent.

globel attributes 
eg:class, id


fragments #

accessibility
THe ability to be accessed and used independently by people no matter their circumstances.

payload
the information, along with the request that the resource can then use if it chooses to do work.

form
the form element reperesnts a hyperlink that can be manipulated through a collection of form-associated elements, some of which can reperesent editable values that can be submitted to a server for processing.

dom maniputation
changing the DOM tree after the HTML document has been parsed and the DOM has been created.



-------------------


day1
Introduction to Internet, Browser, Domain, HTML
1. Understanding Basics of web development
What is Internet
What is Browser
What is Domain
How Internet works
2. Understanding HTML Basics
Introduction to HTML
Role of HTML in web development
Basic structure of an HTML document (<!DOCTYPE html>, <html>, <head>,
<body>)
How to create boiler plate using! Symbol (shortcut to create new HTML
doument with basi tag)
3. Setting Up Your Environment
Choosing a code editor (e.g., VSCode, Sublime Text)
Setting up a basic HTML project
How to Install Extensions like live server, prettier etc
Practice
Create a simple HTML page and using ! Symbol to create basic struture of an
HTML page

day2
Basic Tags Basic Elements and Basic Attributes
1. Basic Tags and Elements, Attributes
Paragraphs (<p>)
Headings (<h1> to <h6>)
Line breaks (<br>)
Emphasis and strong text (<em>, <strong>)
What is HTML attributes?
HTML Class Attribute
How to add a class and How to add multiple classes?
HTML ID Attribute
Why we cannot add multiple id's?
HTML title Attribute
HTML Style Attribute
How many internationalization attributes and which are available for mostly
2. Inline vs. Block Elements
Definition and differences between inline and block elements
Examples of block elements: <div>, <p>, <h1>, etc.
How to add nested div's and How to add nested p tag inside a div tag
Examples of inline elements: <span>, <a>, <img>, etc.

day3
Text Formatting, Lists, Hyperlinks and HTML Comments
1. Text Formatting (1 hour)
Bold (<b>), Italics (<i>)
Underline (<u>), Strikethrough (<s>)
Subscript (<sub>) and Superscript (<sup>)
Quotes and citations (<blockquote>, <cite>)
2. Creating Lists
Unordered lists (<ul>) and list items (<li>)
Ordered lists (<ol>)
Nested lists
Description lists (<dl>, <dt> <dd>)
3. Hyperlinks
Anchor tags (<a>)
Linking to external and internal pages
Email links
Opening links in new tabs with the target attribute
4. HTML Comments and Special Characters
Adding comments (<!-- Comment here -->)
HTML special characters (e.g.,&amp;, &copy;, &nbsp;)
Practice
Build a webpage with links, lists, and formatted text.

day4
Images, Multimedia, and Forms
1. Images
Image tags (<img>)
Adding alt text for accessibility
Image formats and optimization - png, jpeg, webp, svg, avif, etc
Responsive images using srcset
2. Multimedia: Audio and Video
Embedding audio (<audio>)
Embedding video (<video>)
Using the <embed>, <object>, and <iframe> tags
HTML Forms and Advanced form
3. Forms
Form tags (<form>, <input>, <textarea>, <button>)
Input types: text, password, checkbox, radio, etc.
Labels and fieldsets
Form validation basics
1. Advanced HTML Forms
Form validation techniques
Understanding of <datalist>, <fieldset>, <legend>, <optgroup>, <option>,
<output> and <select> tags.
Practice
Design a webpage that includes images, videos, and audio
Build a complex form with validation

day5
Tables
Table tags (<table>, <tr>, <td>, <th>, etc)
Adding borders and styling
Colspan and Rowspan
Understanding of new Table tags <col>, <colgroup>, <thead>, <tbody> and
tfoot> HTML tags.
Practice
Create a table with contents atleast 3 rows and 3 columns
Creating complex tables including new Table tags.

day6
Semantic HTML and HTML5 Features
1. Semantic HTML
Importance of semantic HTML
Semantic elements: <article>, <section>, <aside>, <nav>, <footer> etc
HTML5 semantic tags and their roles in SEO
2. HTML5 Features
New input types: date, color, range, etc.
Placeholder and required attributes
Datalist element for suggestions
Using <progress> and <meter> elements
Practice
Create a webpage with semantic HTML elements and HTML5 input types.


Good to Cover
1.SVG Graphics
Introduction to Scalable Vector Graphics (SVG)
Basic SVG shapes and elements
Embedding SVG into HTML
Styling SVG with CSS
2. Canvas Element
Introduction to <canvas>
Drawing shapes with JavaScript
Basic animations
Comparison of SVG and Canvas
3. HTML Best Practices and Optimization
Writing clean and maintainable code
Using comments effectively
Code validation and debugging
Performance optimization techniques
4.What is SEO, How to implement
5.Language ISO code
6.URL Encoding
7.HTML Layout
8.HTML API (Geo Location, Drag & Drop, Web worker, Web Socket, Web
Storage etc I
