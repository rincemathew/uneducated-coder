
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

#### What is a loop? What are the types of loops in JS?


#### What is the difference between while and for loops?


#### What is the difference between while and do-while loops?


#### What is the difference between break and continue statement?

#### What is the difference between for and for ...if loops in JS?


#### What is the difference between for...of and for...in loop?

#### What is forEach method? Compare it with for...of and for..in loop?

#### When to use for...of loop and when to use forEach method in application?

Loops
1:11:47
