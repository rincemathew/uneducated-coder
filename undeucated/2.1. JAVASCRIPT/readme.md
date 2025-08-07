# JAVSCRIPT


|  content  | topics |
| -----| ----- |
| [**Core JavaScript Concepts**](#core-javascript-concepts) |
| [Variables](#variables) | |
| [Data Types](#data-types) | |
| [undefinded vs null](#undefinded-vs-null) | |
| [Type coercion](#type-coercion) | |
| [scopes](#scopes) | |
| [Lexical scope and Closures](#lexical-scope-and-closures) | |
| [Rest API](#rest-api) | |
| [Rest API](#rest-api) | |
| [Rest API](#rest-api) | |
| [Rest API](#rest-api) | |
| [Rest API](#rest-api) | |
| [**javascript Intermediate Concepts**](#javascript-intermediate-concepts) |
| [**javascript Asynchronous**](#javascript-asynchronous) |
| [What is Callbacks?](#what-is-callbacks-callback-function) | |
| [Rest API](#rest-api) | |


## Core JavaScript Concepts

### Variables
Variables are used to store and manage values that may change throughout your application.
var, let, const

### Data Types
string, number, boolean, null, undefined, symbol, object, functions, array

### undefinded vs null

### Type coercion
1.Implicit corecion
when javascript automatically converts one data type to another.
2.Explicit Corecion
When you deliberately convert one type to another.

### scopes
global scope, local scope, block scope

### Lexical scope and Closures
lexical scope refers to how the scope is determined by where the variables and functions are defined in the code.

closures are used to create functions that can remember their surrounding environment, even after they are executed in a different scope. Closures are commonly used in callbacks, event handlers, and function factories.

` javascript
function createCounter() {
    let count = 0; //'count' is enclosed in 
    return function() {
        count++;   // accessing the count variable from the outer scope
        console.log(count)
    };
}

const counter = createCounter(); //counter is a closure that rememers count
counter();  //output:1
counter();  //output:2
counter();  //output:3
`

### What is Hositing?
Hoisting is Javascrtips default behaviour of moving declarations(not initializations) to the top of their containing scope during the compilation phase, before the code has been executed.

variable hoisting
function hoisting

### Temporal Dead Zone(TDZ)?
When variables are declared with let and const, they do not get intialized until the code execution reaches the declaration. This period is known as the Temporal Dead Zone(TDZ).

question: hoisting with let and const


## javascript Intermediate Concepts

## javascript Asynchronous




### What is Callbacks? (callback function)

A callback is a function that is passed as an argument to another function and is executed after some kind of event or task has completed. Callbacks are used to make sure certain code doesn’t execute until another code has already finished execution. This is particularly useful in asynchronous programming, where actions that take time to complete, such as data fetching or file I/O, are involved.

`javascript
function fetchData(callback) {
    setTimeout(function() {
        console.log("Data fetched");
        callback(); // Call the callback function
    }, 2000);
}

function processData() {
    console.log("Processing data");
}

// fetchData is called with processData as a callback
fetchData(processData);

`
output

`
Data fetched
Processing data
`

Example in event Handling
`javascript
document.getElementById("myButton").addEventListener("click", function() {
    console.log("Button was clicked!");
});
//the function passed to addEventListener is a callback function that will be executed when the "click" event occurs on the element with the id "myButton".
`

### Why Use Callbacks?
1. Asynchronous Operations: Callbacks allow you to handle asynchronous operations like HTTP requests, reading files, etc., without blocking the execution of other code.
2. Decoupling: They help in decoupling the function execution from the function definition. You can pass different functions as callbacks to achieve different behaviors.
3. Event Handling: Callbacks are extensively used in event-driven programming, such as handling user interactions in a web application.

### Synchronous vs. Asynchronous Callbacks
Synchronous Callbacks: These are executed immediately and block the execution of the next line of code until they are finished.

`javascript
function greet(name, callback) {
    console.log("Hello " + name);
    callback();
}

function sayGoodbye() {
    console.log("Goodbye!");
}

greet("Alice", sayGoodbye);

`
output
`
Hello Alice
Goodbye!

`

Asynchronous Callbacks: These are executed after an asynchronous operation has been completed, allowing the rest of the code to run during the waiting period.

`
function fetchData(callback) {
    setTimeout(function() {
        console.log("Data fetched");
        callback(); // Call the callback function
    }, 2000);
}

function processData() {
    console.log("Processing data");
}

fetchData(processData);
`
Output
`
Data fetched
Processing data
`







js is event based language

callback hell

promise
used for asynchronous function
resolve reject pending

```
code 
```

promise chaining
catch and utils functions(resolve reject all race)
try catch finally throw 
async await
event bloking




`````````
1
what is javascript
history
ecmascript

include script in html
async defer