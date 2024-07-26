What is a View engine?
A template engine enables you to use static template files in your application. At runtime, the template engine replaces variables in a template file with actual values and transforms the template into an HTML file sent to the client. This approach makes it easier to design an HTML page.

A response is rendered when a request is sent to the homepage. It selects an EJS file (in our case, myEJS.ejs) as a template to which arguments are passed from the Javascript file. This lets us create multiple HTML pages using the same base template. They may, however, have different values to be passed to them.

views, the directory where the template files are located. Eg: app.set('views', './views'). This defaults to the views directory in the application root directory.
view engine, the template engine to use. For example, to use the Pug template engine: app.set('view engine', 'pug').
Some popular template engines that work with Express are Pug, Mustache,Handlebars and EJS


EJS - embedded javascript
Ejs allows us to run plain js in HTML
Ejs simple, light weight, fast
Most popular


<% 'Scriptlet' tag, for control-flow, no output
<%_ ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it
<%= Outputs the value into the template (HTML escaped) -escapes the html tags, and does not let them to be translated.
<%- Outputs the unescaped value into the template -where html is translated (unescaped), and you see the result you wish.
<%# Comment tag, no execution, no output
<%% Outputs a literal '<%'
%> Plain ending tag
-%> Trim-mode ('newline slurp') tag, trims following newline
_%> ‘Whitespace Slurping’ ending tag, removes all whitespace after it

