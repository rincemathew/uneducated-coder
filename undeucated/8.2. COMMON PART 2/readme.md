# Common in Computer Science

### AJAX (Asynchronous javascript and XML)
AJAX is not a programming language. It's a technology for developing better, faster and more interactive web applications using HTML, CSS, JS, and XML.
Asynchronous means the web application can send and receive data from the web server without refreshing the page. This background process of sending and receiving data from the server along with updating different sections of a web page defines the features of Ajax.
AJAX makes use of a browser build-in XMLHttpRequest object to request data from a Web Server and HTML DOM to display or use the data.

function changeContent() {
  var xhttp = new XMLHttpRequest();
  xhttp.onreadystatechange = function() {
    if (this.readyState == 4 && this.status == 200) {
     document.getElementById("foo").innerHTML = this.responseText;
    }
  };
  xhttp.open("GET", "content.txt", true);
  xhttp.send();
}

Many modern web applications still use AJAX, but it's worth mentioning that newer technologies like Fetch API and async/await in JavaScript have become popular and offer more modern and flexible ways to handle asynchronous operations. The Fetch API, for example, is a native JavaScript API for making HTTP requests and is often considered a more modern alternative to traditional AJAX.


### XML
XML (Extensible Markup Language) is a markup language similar to HTML, but without predefined tags to use. Instead, you define your own tags designed specifically for your needs. This is a powerful way to store data in a format that can be stored, searched, and shared. Most importantly, since the fundamental format of XML is standardized, if you share or transmit XML across systems or platforms, either locally or over the internet, the recipient can still parse the data due to the standardized XML syntax.
There are many languages based on XML, including XHTML, MathML, SVG, RSS, and RDF. You can also define your own.

### JSON
JSON stands for JavaScript Object Notation. JSON is a lightweight data interchange format. It's easy for humans to read and write. It's easy for machines to parse and generate.
*Converting JSON string into Javascript object - JSON.parse()
*object into a JSON string - JSON.stringify()

##HTTP status Codes
Used for authentication401 not authorization403


vite
alternative to CRA

in CRA it bundles all your JS modules, CSS and other assets every time you make a change that slows the bundling when the app grows.
in Vite  it takes advantage of native ES modules nad serves ditectly to the browser.
Hot module replacement



tailwind CSS
Utility first approach
responsive design
customization
dark mode support
optimized production build



ASCII-based plain text are being replaced with Unicode as a universal character encoding.