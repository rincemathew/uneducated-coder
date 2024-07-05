# JAVSCRIPT

## javascript basics

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