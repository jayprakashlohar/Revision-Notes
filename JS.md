## HTML,CSS And JavaScript Basic



## What is data structure explain?
_A data structure is a specialized format for organizing, processing, retrieving and storing data. There are several basic and advanced types of data structures, all designed to arrange data to suit a specific purpose. Data structures make it easy for users to access and work with the data they need in appropriate ways._

## What is an Array?
_An array is a collection of items of same data type stored at contiguous memory locations.
This makes it easier to calculate the position of each element by simply adding an offset to a base value, i.e., the memory location of the first element of the array (generally denoted by the name of the array). The base value is index 0 and the difference between the two indexes is the offset._

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

The below example creates a throttle function to reduce the number of events
 for each pixel change and trigger scroll event for each 100ms except for the first event.*

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

 ## What is the difference between a block element and an inline element? 
 ## Give few examples of block and inline tags which we have in HTML.
 
A block element is a type of HTML element that creates a “block” of space on a page, 
meaning that it takes up the full width available and automatically starts a new line after it. Block elements can contain other block and inline elements. Examples of block elements are: 

<h1>, <p>, <div>, <ul>, <table>, <form>, <header>, <footer>, <blockquote>, <pre>.

An inline element is a type of HTML element that only takes
 up as much width as necessary and does not automatically start a new line. Inline elements can only contain other inline elements and cannot contain block elements. Examples of inline elements are: 

<a>, <span>, <strong>, <img>, <input>, <em>, <label>, <button>.

## What are pseudo-elements and pseudo-classes in CSS? Give some examples.
Pseudo-elements and pseudo-classes in CSS are used to target specific elements on 
a web page. They allow you to style elements with CSS without having to add additional HTML markup.

Pseudo-elements are used to style specific parts of an element, such as the first
 letter of a paragraph or the first line of a blockquote. 
 Examples of pseudo-elements include ::first-line, ::first-letter, and ::before.

Pseudo-classes are used to style elements based on their state or position
 in the document. Examples of pseudo-classes include :hover, :active, 
 :visited, :focus, :first-child, and :last-child.

## What are CSS positions? What are the position types in CSS? What is the default position property in CSS?

CSS positions are the values used to define the position of
 an element in a web page. The position types in CSS are static,
  relative, absolute, fixed, and sticky. The default position property in CSS is static.

## What is difference between Local storage, session storage and cookies?
Local Storage: Local storage stores data with no expiration date. 
The data will not be deleted when the browser is closed, and will be available the next day, week, or year.

Session Storage: Session storage stores data for a single session (the data is deleted when the browser tab is closed).

Cookies: Cookies are small pieces of data sent from a website and 
stored in a user’s web browser while the user is browsing that website. 
Cookies are primarily used to track a user’s activities while they are on
 the website, such as what pages they have visited, what items they have added 
 to their shopping cart, etc. Cookies are also used to store user preferences and
  login information. Unlike local storage and session storage, cookies are sent 
  back and forth between the browser and the server with each request.

## What are different higher order functions in JS? What is the difference between .map() and .forEach() ?

1. Higher order functions in JS include filter(), map(), reduce(), forEach(), and some. 
2. The difference between .map() and .forEach() is that .map() returns a 
new array with the results of calling a provided function on every element
 in the given array, while .forEach() calls a provided function once for 
 each element in an array, in order. .map() is usually used when you want 
 to transform data from one type to another, while .forEach() is usually used when you want to execute a set of instructions on each element in an array.

## What is Hoisting in Javascript?

Hoisting is a JavaScript mechanism where variables and function declarations 
are moved to the top of their scope before code execution. In JavaScript, 
a variable can be declared after it has been used. In other words,
 a variable can be used before it has been declared. Hoisting is JavaScript's 
 default behavior of moving declarations to the top.

## What are promises? What are the different states of a promise?
## Support your answer with an example where you need to create your own promise.

Promises are objects that represent the eventual completion (or failure) of
 an asynchronous operation, and its resulting value. Promises are used to handle 
 asynchronous operations in JavaScript, allowing you to write synchronous-looking code that still works asynchronously.

The different states of a promise are:
1. Pending: The initial state of a promise, indicating that the operation has not yet completed.
2. Fulfilled: The state of a promise representing a successful operation.
3. Rejected: The state of a promise representing a failed operation.

Example: 

let myPromise = new Promise((resolve, reject) => {
    // do some asynchronous work
    if (/* asynchronous work successful */) {
        resolve('Success!');
    } else {
        reject('Error!');
    }
});

## What is ‘this’ keyword in JavaScript? explain with an example

The 'this' keyword in JavaScript is used as a reference to the object that is currently executing a method. It is a very powerful keyword as it can be used to refer to the current object, its parent object, or the global object.

For example, if we have a function called 'myFunction' inside an object called 'myObject', we can refer to the object itself using the 'this' keyword inside the 'myFunction' function: 

const myObject = {
  name: 'John',
  myFunction: function() {
    console.log(`My name is ${this.name}`)
  }
};

myObject.myFunction(); // My name is John


