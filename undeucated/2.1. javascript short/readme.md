
---------------------
#### what is javascript?
javascript is a programming laguage that is used for converting static web pages to interactive and dynamic web pages.

#### what is the role of javascript engine?
a javascript engine is program present in web browsers that executes javascript code

#### different types of javascript engines
v8 - chrome
spider monkey - firefox
javascript core - safari
chakra - edge

#### different methods to add javascript code into html file
<script></script>
<script src="index.js"></script>


#### what is client side?
a client is a device, application, or software component that requests and consumes services or resources from a server.

#### what is server side?
a server is a device, computer or software application that provides services, resouces, or functions to client.

#### what is scope is javascript?
scope determines where varibales are defined and where they can be accessed.
global, function, block


#### what is the type of a variable in JS when it is declared without using the var, let or const keywords?
"var is the implicit type of variable when a variable is declared without var, let, or const keywords

#### what is Hoisting in Javascript?
Hoisting is a Javascript behaviour where functions and variables declarations are movied to the top of their respective scopes during the compilation phase.

#### what is JSON?
Javascript object Notation is a lightweight data interchange format.
JSON consists of key-value pairs

#### what are variables?
variables are used to store data.

#### what is the difference between var, let and const?
var creates a function-scoped variable
let creates a block-scoped variable
const can be assigned only once and its value cannot be changes afterwards.

#### What are data types in JS?
a data type determines the type of variable.
primitive=numbers,string,booleans,undefined,null
non-primitive=object,array,function,date,regexp

#### what is the difference between primitive and non-primitive data types?
primitive data types can hold only single value
Primitive date types are immutable, meaning their values, once assigned, cannot be changed
Non -primitive data types can hold multiple value,
Type are mutable and their values can be changed.

#### What is the difference between null and undefined in JS?
When a variable is declared but has not been assigned a value, its automatically initalized with undefined.
Null varibale are intentionally assigned the null value.

#### what is the use of typeof operator?
typeof operator is user to determine the type of each variable.

#### What is type coercion in JS?
Type coercion is the automatic conversion of values from one data type to anoter during certain operations or comparisons.

### What is operator precedence?
As per operator precedence, operators with higher precedence are evaluated first. (BODMAS)

#### What are operators? What are the types of operators in JS?


#### What is the difference between unary, binary and ternary operators?

#### What is short-circuit evaluation in JS?
short-circuit evaluation stops the execution as soon as the result can be determined witout evaluating the remaining sub-expressions.

#### What are the types of conditions statements in JS?
if/else statement
Ternary operator
Switch statement

#### When to use which type of conditions statements in real applications?
if/else statement - 
Ternary operator - 
Switch statement - 

#### What is the difference between == and ===?
Loose Equality(==) operator compares two values for  equality after performing type coercion.

Strict equality(===) operator compares two values for equality witout performing type corecion.

#### What is the differnce between Spread and rest operatior in JS?
The spread operator(...) is used to expand or spread elements from an iterable(such as an array, string, or object) into individual elements.
##### use of spread operator
Copying an Array
Merging Arrays
Passing multiple arguments to a function

The rest operator is used in function parameters to collect all remainging arguments into an array.

#### What are Arrays in JS? How to get, add and remove elements from arrays?
An array is a data type that allows you to store multiple values in a single variable.
Get - indexOf(), find(), filter(), slice()
Add - push(), concat()
Remove - pop(), shift(), splice()
Modify - map(), forEach()
others - join(), length, sort(), reverse(), reduce(), some(), every()

#### What is the indexOf() method of an Array?
indexOf() method gets the index of a specified element in the array.

#### What is the difference between find() and filter() methods of an Array?
find() method get the first element that satisfies a condition.
filter() method get an array of elements that satisfies a condition.

#### What is the slice() method of an Array?
slice() method get a subset of the arry from start index to end index(end not included)

#### What is the difference between push() and concat() methods of an Array?
Push() will modify the original array itself.
concat() method will create the new array and not modify the original array.

#### What is the difference between pop() and shift() methods of an Array?
pop() will remove the last element of the array.
shift() will remove the first element of the array.

#### What is the splice() method of an Array?
The splice() method is used to addd, remove, or replace elements in an array.

#### What is the differnce between slice() and splice() methods of an Array?
THe slice() method is used get a subset of the array from the start index to the end index(end not included)
The splice() method is used to addd, remove, or replace elements in an array.

#### What is the differnce between map() nad forEach() array methods?
The map() method is used when you want to modify each element of array and create a new array with the modified values.
The forEach() method is used when you want to perform some operation on each element of an array without creating a new array.

#### How to sort and reverse an array?
Array can be sorted or reversed by using sort() and reverse() methods of array.

#### What is Array Destructuring in JS?
Array destructuring allows you to extract elements from an array and assign them to individual variables in a single statement.

#### What are arry-like objects in JS?
Array-like object are objects that have indexed elements and a length property, similar to arrays, but they may not have all the methods of arrays like push(), pop() and others
eg:arguments, strings, HTML collections.

#### How to convert and array-like object into an Array?
Array.from()
Spread syntax (...)
Array.prototype.slice.call()

### loops

#### What is a loop? What are the types of loops in JS?
A loop is programming way to run a piece of code repeatedly untile a certain condition is met.
JS loops - for, while, do-while, for-of, for-in

#### What is the difference between while and for loops?
for loop allows to iterate a block of code a specific number of times.

while loop execute a block of code while a certain condition is true.

#### What is the difference between while and do-while loops?
while loop execute a block of code while a certain condition is true.

The do-while loop is similar to the while loop, except that the block of code is executed at least once, even if the codition is false.

#### What is the difference between break and continue statement?
The break statement is used to terminate the loop.
the continue statement is used to skip the current iteration of the loop and move on to the next iteration.

#### What is the difference between for and for ...if loops in JS?


#### What is the difference between for...of and for...in loop?
for..of loop is used to loop through the values of an object like arrays,strings.
it allows you to access each value directly without having to use an index.

for...in loop is used to loop through the properties if an object.
it allows you to iterate over the keys of an object and access the values associated by using keys as the index.

#### What is forEach method? Compare it with for...of and for..in loop?
forEach() is a method available on arrays or object that allows you to iterate over each element of the array and perform some action on each element.

#### When to use for...of loop and when to use forEach method in application?
for..of loops is suitable when you need more control over the loop, such as using break statement or continue statement inside.

forEach method iterate over each element of the array and perform some action on each element.

#### What are functions is JS? what are the types of functions?
A function is a reusable block of code that performs a specific task.

types - Names function, Anonymous function, function expression, Arrow Function, IIFE, Callback Function, Higher-Order Function.

#### What is the difference between named and anonymous functions? when to use what is applications?
Named Functions have a name identifier.
use named functions for big and complex logics.
Use when you want to reuse one function at multiple places.

Anonymous functions do not have a name identifier and cannot be referenced directly by name.
Use anonymous functions for small logics.
Use when want to use a function in a single place.

#### What is function expressions in JS?
A function expression is a way to define a function by assigning it to a variable.

#### What are Arrow funtions in JS? What is it use?
Arrow functions, also know as fat arrow functions, is a simpler and shorter way for defining functions in Javascript.

#### What are Callback functions? What is it use?
A callback function is a function that is passed as an argument to another function.

#### What is Higher-order function in JS?
Take one or more functions as arguments or Return a function as a result.

#### What is the difference between arguments and parameters?
Parameters are the placeholders defined in the function declaration.

Arguments are the actual values passed to a function when it is invoked or called.

#### in how many ways can you pass arguments to a function?
positional arguments
Named arguments
arguments object

#### How do you use default parameters in a function?
In javascript, default parameters allow you to specify default values for function parameters.

#### What is the use of event handling in JS?
Event handling is the process of responding to user actions in a web page.
The addEventListener method of javascript allows to attach an event name and with the function you want to perform on that event.

#### What are First-Class functions in JS?
A programming language is said to have First-class functions if functions in that languages are trated like other varibales.

like Assignable, passable as Arguments, returnable as values

#### What are Pure and Impure functions in JS?
A pure function is a function that always produces the same output for the same input.
Pure functions cannot modify the state.
Pure functions cannot have side effects.

An impure functions, can produce different outputs for the same input.
Impure functions can modify the state.
Impure functions can have side effects.

#### What is Function Curring in JS?
Curring in Javascript transofroms a function with multiple arguments into a nested seried of functions, each taking a single arguemnt.

Advantage: Reusability, modularity and specialization. Big, complex functions with multiple argumets can be broken down into small, reusable functions with fewer arguments.

#### What are call, apply, bind methods in JS?
call, apply and bind are three methods in javascript that are used to work with functions and control how they are invoked and what cotext they operate in.

These methods provide a way to manipulate the this value and pass arguments to functions.


#### string
#### What is a String?
A string is a data type used to store and manipulate date.

#### What are template literals and string interpolation in strings.
 ${} - A template literal, also know as a template string, is a feature introduced in ECMAScript 2015(ES6) for string interpolation and multiline strings in Javascript

#### what are the different between single quote (') double quote ("") and back ticks (``)

#### What are some important string operations in JS?
substr(), substring()..........................

#### What is string immutability?


#### In how many ways you can concatenate strings?
+operator, concat() method, template literals, join() method


#### DOM

#### What is DOM? What is the difference between HTML and DOM?

#### How do you select, modify, create and remove DOM elements?

#### What are selectors in JS?

#### What is the differnce between getElementById, getElementsByClassName and getElementsByTagName?

#### What is the difference between querySelector() and querySelectorAll()?

#### What are the methods to modify elements properties and attributes?

#### What is the difference between innerHTML and textContent?

#### How to add and remove properties of HTML elements in the DOM using JS?

#### How to add and remove properties of HTML elements in the DOM using JS?

#### How to add and remove style from HTML elements in DOM using JS?

#### How to create new elements in DOM using JS? What is the dofference between createElement() and cloneNode()?

#### What is the difference between createElement() and createTextNode()?

#### Error handling

#### What is Error Handling in JS?

#### What is the role of finally block in JS?

#### What is the purpose of the throw statement in JS?

#### What is Error propagation in JS?

#### What are the best practices for error handling?

#### What are the different types of errors in JS?

#### What are objects in JS?

#### In how many ways we can create an object?

#### What is the difference between an array and an object?

#### What is the difference between array and objects?

#### How do you add or modify or delete properties of and object?

#### Explain the difference between dot notation and bracket notation?

#### What are some common methods to iterate over the properties of an object?

#### How do you check if a property exists in an object?

#### How do you clone or copy an object?

#### What is the difference between deep copy and shallow copy on JS?

#### What is Set Object in JS?

#### What is Map Object in JS?

#### What is the differnce between Map and Object in JS?

#### Events
#### What are Events?  How are events triggered?

#### What are the types of events in JS?

#### What is Event Object in JS?

#### What is Event Delegation in JS?

#### What is Event Bubbling in JS?

#### How can you stop event propagation or event bubbling in JS?

#### What is Event Capturing in JS?

#### What is the purpose of the event.preventDefault() method in JS?

#### What is the use of "this" keyword in the context of event handling in JS?

#### How to remove an event handler from an element in JS?




2:02:00
