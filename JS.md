## HTML,CSS And JavaScript Basic

## What is data structure explain?
_A data structure is a specialized format for organizing, processing, retrieving and storing data. There are several basic and advanced types of data structures, all designed to arrange data to suit a specific purpose. Data structures make it easy for users to access and work with the data they need in appropriate ways._

## What is an Array?
_An array is a collection of items of same data type stored at contiguous memory locations.
This makes it easier to calculate the position of each element by simply adding an offset to a base value, i.e., the memory location of the first element of the array (generally denoted by the name of the array). The base value is index 0 and the difference between the two indexes is the offset.

##  what is self closing tag in html?
_Some HTML tags (like img and br ) don't have their own content. These are known as self closing tags or empty tags. They look like this: A simple example: <br /> The br tag inserts a line break (not a paragraph break)._

## what is default value of position property?
_CSS Position: Static Value
This is the default value for the CSS position property. In this mode, the target element is positioned along with the natural document flow. Note that the top, right, bottom, left, as well as z-index properties will not display any effects_

## What is a setAttribute in JavaScript?
_The setAttribute() method sets a new value to an attribute. If the attribute does not exist, it is created first._
_element.setAttribute("class", "democlass");_

## What is a settimeout in js?
_The global setTimeout() method sets a timer which executes a function or specified piece of code once the timer expires._
EXAMLE -
_setTimeout(() => {
console.log("Delayed for 1 second.");
}, 1000)_

## what is setinterval in javascript?
_The setInterval() function is commonly used to set a delay for functions that are executed again and again, such as animations. You can cancel the interval using clearInterval() _
EXAMLE -
\*const intervalID = setInterval(myCallback, 500, 'Parameter 1', 'Parameter 2');

function myCallback(a, b)
{
// Your code here
// Parameters are purely optional.
console.log(a);
console.log(b);
}\*

## Window clearInterval()?
_Display the time once every second. Use clearInterval() to stop the time:_
EXAMLE -
\*const myInterval = setInterval(setColor, 500);

function setColor() {
let x = document.body;
x.style.backgroundColor = x.style.backgroundColor == "yellow" ? "pink" : "yellow";
}

function stopColor() {
clearInterval(myInterval);
}\*

## HTTP Methods?
_GET
POST
PUT
HEAD
DELETE
PATCH
OPTIONS
CONNECT
TRACE_

## What is HTTP?
_The Hypertext Transfer Protocol (HTTP) is designed to enable communications between clients and servers.
HTTP works as a request-response protocol between a client and server.
Example: A client (browser) sends an HTTP request to the server; then the server returns a response to the client._

## Diffrent between HTTP AND HTTPS IN JS ?

- 1. HyperText Transfer Protocol (HTTP): HyperText Transfer Protocol (HTTP) is a protocol using which
 hypertext is transferred over the Web. Due to its simplicity, http has been the most widely used protocol
  for data transfer over the Web but the data (i.e. hypertext) exchanged using http isn’t as secure as we 
  would like it to be. In fact, hyper-text exchanged using http goes as plain text i.e. anyone between the
   browser and server can read it relatively easily if one intercepts this exchange of data.

2. Hypertext Transfer Protocol Secure (HTTPS): Hypertext Transfer Protocol Secure (HTTPS) is
 an extension of the Hypertext Transfer Protocol (HTTP). It is used for secure communication. 
 In HTTPS, the communication protocol is encrypted using Transport Layer Security. \*

\*S.No. HTTP HTTPS

1. HTTP stands for HyperText Transfer Protocol. HTTPS for HyperText Transfer Protocol Secure.
2. In HTTP, URL begins with “http://”. In HTTPs, URL starts with “https://”.
3. HTTP uses port number 80 for communication. HTTPs uses 443 port number for communication.
4. HTTP is considered to be unsecure. HTTPs is considered as secure.
5. HTTP works at Application Layer. HTTPS works at Transport Layer.
6. In HTTP, Encryption is absent. Encryption is present in HTTPS.
7. HTTP does not require any certificates. HTTPS needs SSL Certificates.
8. HTTP does not improve search ranking HTTPS helps to improve search ranking
9. HTTP faster than HTTPS HTTPS slower than HTTP
10. HTTP does not use data hashtags to secure data. While HTTPS will have the data before sending it 
and return it to its original state on the receiver side.\*

## What is promiss ?
\*A Promise is a proxy for a value not necessarily known when the promise is created. 
It allows you to associate handlers with an asynchronous action's eventual success value or 
failure reason. This lets asynchronous methods return values like synchronous methods: 
instead of immediately returning the final value, the asynchronous method returns a promise to 
supply the value at some point in the future.

A Promise is in one of these states:

pending: initial state, neither fulfilled nor rejected.
fulfilled: meaning that the operation was completed successfully.
rejected: meaning that the operation failed.\*

## What are closures
A closure is the combination of a function and the lexical environment within which that function 
was declared. i.e, It is an inner function that has access to the outer or enclosing function’s variables.
 The closure has three scope chains

Own scope where variables defined between its curly brackets
Outer function’s variables
Global variables
Let's take an example of closure concept,

function Welcome(name) {
var greetingInfo = function (message) {
console.log(message + " " + name);
};
return greetingInfo;
}
var myFunction = Welcome("John");
myFunction("Welcome "); //Output: Welcome John
myFunction("Hello Mr."); //output: Hello Mr.John
As per the above code, the inner function(i.e, greetingInfo) has access to the variables
 in the outer function scope(i.e, Welcome) even after the outer function has returned.

## What is scope in javascript

_Scope is the accessibility of variables, functions, and objects in some particular part of your code during runtime. In other words, scope determines the visibility of variables and other resources in areas of your code._

## what is a promise
A promise is an object that may produce a single value some time in the future with either a resolved value or a reason that it’s not resolved(for example, network error). It will be in one of the 3 possible states: fulfilled, rejected, or pending.

The syntax of Promise creation looks like below,

const promise = new Promise(function (resolve, reject) {
// promise description
});
The usage of a promise would be as below,

const promise = new Promise(
(resolve) => {
setTimeout(() => {
resolve("I'm a Promise!");
}, 5000);
},
(reject) => {}
);

promise.then((value) => console.log(value));

## What are the three states of promise
Promises have three states:

*Pending: This is an initial state of the Promise before an operation begins
Fulfilled: This state indicates that the specified operation was completed.
Rejected: This state indicates that the operation did not complete. In this case an error value will be thrown.*

## What is a callback function##
  *A callback function is a function passed into another function as an argument. This function is invoked inside the outer function to complete an action. Let's take a simple example of how to use callback function

function callbackFunction(name) {
  console.log("Hello " + name);
}

function outerFunction(callback) {
  let name = prompt("Please enter your name.");
  callback(name);
}

outerFunction(callbackFunction) *

## What is the use of setInterval
*The setInterval() method is used to call a function or evaluate an expression at specified intervals (in milliseconds). For example, let's log a message after 2 seconds using setInterval method,

setInterval(function () {
  console.log("Good morning");
}, 2000);*


## What is JSON
*JSON (JavaScript Object Notation) is a lightweight format that is used for data interchanging. It is based on a subset of JavaScript language in the way objects are built in JavaScript.*

## What is the purpose of clearTimeout method
*The clearTimeout() function is used in javascript to clear the timeout which has been set by setTimeout()function before that. i.e, The return value of setTimeout() function is stored in a variable and it’s passed into the clearTimeout() function to clear the timer.

For example, the below setTimeout method is used to display the message after 3 seconds. This timeout can be cleared by the clearTimeout() method.

<script>
var msg;
function greeting() {
   alert('Good morning');
}
function start() {
  msg =setTimeout(greeting, 3000);

}

function stop() {
    clearTimeout(msg);
}
</script>*

## What is throttling?
*Throttling is a technique used to limit the execution of an event handler 
function, even when this event triggers continuously due to user actions. The common use cases are browser resizing, window scrolling etc.

## What is debouncing?
*Debouncing is a programming pattern that allows delaying execution of 
some piece of code until a specified time to avoid unnecessary CPU cycles, API calls and improve performance. The debounce function make sure that your code is only triggered once per user 
input. The common usecases are Search box suggestions, text-field auto-saves,
and eliminating double-button clicks.*

### What are the differences between primitives and non-primitives?

*A primitive type has always a value, while non-primitive types can be null .
 A primitive type starts with a lowercase letter, while non-primitive types starts 
 with an uppercase letter. The size of a primitive type depends on the data type, while non-primitive types have all the same size.*

Primitive data - Integer, Float, Boolean, Character
Non-primitive - Array, String, Stack, Queue

## Types of Errors
*
Syntax Error: When a user makes a mistake in the pre-defined syntax of a programming language, a syntax error may appear.
Runtime Error: When an error occurs during the execution of the program, such an error is known as Runtime error. The codes which create runtime errors are known as Exceptions. Thus, exception handlers are used for handling runtime errors.
InternalError: It creates an instance when the js engine throws an internal error.
RangeError: It creates an instance for the error that occurs when a numeric variable or parameter is out of its valid range.
ReferenceError: It creates an instance for the error that occurs when an invalid reference is de-referenced.
SyntaxError: An instance is created for the syntax error that may occur while parsing the eval().
TypeError: When a variable is not a valid type, an instance is created for such an error.*


### Hoisting *is a concept which enables us to extract values of variables and functions even before initialising/assigning value without getting error and this is 
 ## happening due to the 1st phase (memory creation phase) of the Execution Context.*

## Synchronous JavaScript:
 *As the name suggests synchronous means to be in a sequence, i.e.
  every statement of the code gets executed one by one. So, basically a statement has to wait for the earlier statement to get executed.*

 ## Asynchronous way: 
 It never waits for each operation to complete, rather it
  executes all operations in the first only. The result of each operation will be handled once the result is available*




### SOME MORE JS QUESTION 

## difference between var let const ?

Var, Let, and Const are all used to declare variables in JavaScript.
Var is used for globally scoped or function scoped variables.
Let is used for block scoped variables.
Const is used for block scoped variables that are read-only and cannot be reassigned.

## spread operator?
The spread operator (...) is used to expand elements in an iterable object, such as an array, into a list of arguments. It can be used to spread elements of an array into a function's arguments, or to spread an array into another array.

## what is rest operator ?
The Rest Operator is a syntax used in JavaScript to create a new array out of the existing array's elements, excluding the last one. The operator is represented by three dots (...) and it is used to gather all remaining elements into an array. It can also be used to pass an indefinite number of arguments to a function.

## what is Arrow function ?
Arrow functions are a new syntax for writing JavaScript functions. They are shorter and more concise than traditional function expressions and are best suited for non-method functions. Arrow functions do not have their own this, arguments, super, or new. target bindings.

## what is Destructuring ?
Destructuring is a feature of JavaScript that allows you to extract values from arrays and objects and assign them to variables. It helps simplify code by allowing you to quickly assign values to variables without having to write multiple lines of code.

## what is Default Params?
Default params are parameters that are given a default value if no other value is specified when a function is called. It allows a function to be called without arguments, or with only some of the arguments specified.

## what is Template Literals ?
Template Literals are strings that allow embedded expressions. They are surrounded by backticks (` `) and can contain placeholders which are represented using ${expression}. Template literals can be used for string interpolation and multi-line strings.
## what is Optional Chaining?
Optional chaining is a feature in JavaScript that allows developers to access, assign, and invoke objects, properties, and methods safely and with ease. It is used to prevent errors by allowing them to write code without having to check whether a property or method exists. Optional chaining simplifies the syntax of dealing with nested objects and prevents having to write code to handle undefined values.

## Classes in js?
In JavaScript, classes are special functions that can be used to create objects and define their properties and methods. Classes provide a much cleaner and simpler way to create objects with their own properties and methods, compared to object literals or constructor functions.

## 