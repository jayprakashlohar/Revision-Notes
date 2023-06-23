## What is the difference between a block element and an inline element? Give few examples of block and inline tags which we have in HTML.

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

## What are promises? What are the different states of a promise? Support your answer with an example where you need to create your own promise.

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
if (/_ asynchronous work successful _/) {
resolve('Success!');
} else {
reject('Error!');
}
});

## What is ‘this’ keyword in JavaScript? explain with an example?

The 'this' keyword in JavaScript is used as a reference to the object that is currently executing a method. It is a very powerful keyword as it can be used to refer to the current object, its parent object, or the global object.

For example, if we have a function called 'myFunction' inside an object called 'myObject', we can refer to the object itself using the 'this' keyword inside the 'myFunction' function:

const myObject = {
name: 'John',
myFunction: function() {
console.log(`My name is ${this.name}`)
}
};

myObject.myFunction(); // My name is John

<!-- ------------------------------------- Some More Important Question --------------------------------- -->

## What is the difference between Java and Javascript?

Java is a general-purpose programming language used for building applications, while JavaScript is primarily used for web development and adding interactivity to web pages.

Java has a C-style syntax, requires explicit type declarations, and runs on the Java Virtual Machine (JVM). JavaScript has a more flexible syntax, is dynamically typed, and is executed by web browsers.

Java is class-based, while JavaScript follows a prototype-based model.

Java has an extensive standard library, while JavaScript's standard library is smaller but can be extended with libraries and frameworks.

## What are the different primitive data types in JS?

Number: Represents numeric values, including integers and floating-point numbers. For example: 10, 3.14.

String: Represents a sequence of characters enclosed in single quotes (') or double quotes ("). For example: 'Hello', "JavaScript".

Boolean: Represents a logical value, either true or false. It is often used for conditional statements and comparisons.

Null: Represents the intentional absence of any object value. It is a special value that signifies the absence of a value.

Undefined: Represents an uninitialized or unassigned value. If a variable is declared but not assigned a value, it is undefined by default.

Symbol: Introduced in ECMAScript 6, symbols are unique and immutable data types used for creating unique identifiers. Symbols are often used as keys for object properties to avoid name collisions.

These primitive data types are immutable, which means their values cannot be modified. JavaScript also has a special object type, which is not a primitive data type but is used to store collections of key-value pairs.

## What is the difference between null, undefined, and NaN?

null: It is a value that represents the intentional absence of any object value. It is often used to indicate that a variable or object property has no assigned value. When a variable is explicitly set to null, it means that it has no value or points to no object. It is a primitive type.

undefined: It represents an uninitialized or unassigned value. When a variable is declared but not assigned a value, or when an object property does not exist, its value is undefined. It is often used to indicate the absence of a meaningful value. It is a primitive type.

NaN: It stands for "Not a Number" and represents a value that is not a valid number. It is typically the result of an arithmetic operation that could not produce a meaningful numeric value. For example, dividing zero by zero or performing mathematical operations on non-numeric values will result in NaN. It is a special value of the Number type.

To summarize, null is an intentional absence of an object value, undefined indicates an uninitialized value, and NaN represents a value that is not a valid number.

## What are higher-order functions? What are callbacks?

Higher-order functions: In JavaScript, a higher-order function is a function that can receive another function as an argument and/or return a function as its result. In other words, it treats functions as first-class citizens. Higher-order functions enable powerful functional programming techniques and abstraction.

Callbacks: A callback is a function that is passed as an argument to another function and is executed later in the execution flow. Callback functions are commonly used in asynchronous operations, event handling, and higher-order functions. The receiving function can "call back" or invoke the callback function at the appropriate time, often with specific arguments or data.

Higher-order functions and callbacks work together to achieve dynamic and flexible behavior in JavaScript. Higher-order functions allow functions to be manipulated and composed, while callbacks provide a way to specify custom behavior to be executed at a certain point in a function's execution or in response to an event.

## What are higher-order functions? What are callbacks?

Higher-order functions: In JavaScript, a higher-order function is a function that can receive another function as an argument and/or return a function as its result. In other words, it treats functions as first-class citizens. Higher-order functions enable powerful functional programming techniques and abstraction.

Callbacks: A callback is a function that is passed as an argument to another function and is executed later in the execution flow. Callback functions are commonly used in asynchronous operations, event handling, and higher-order functions. The receiving function can "call back" or invoke the callback function at the appropriate time, often with specific arguments or data.

Higher-order functions and callbacks work together to achieve dynamic and flexible behavior in JavaScript. Higher-order functions allow functions to be manipulated and composed, while callbacks provide a way to specify custom behavior to be executed at a certain point in a function's execution or in response to an event.

### Array

## What are the different ways to initialise an Array?

const myArray = [1, 2, 3];
const myArray = new Array(1, 2, 3);
const myArray = new Array(3);
const myArray = Array.from([1, 2, 3]);
const myArray = [...anotherArray];

## Can you create, transpose a matrix. etc?

const matrix = [
[1, 2, 3],
[4, 5, 6],
[7, 8, 9]
];

function transposeMatrix(matrix) {
const rows = matrix.length;
const columns = matrix[0].length;

// Create a new transposed matrix
const transposedMatrix = [];

for (let i = 0; i < columns; i++) {
transposedMatrix[i] = [];
for (let j = 0; j < rows; j++) {
transposedMatrix[i][j] = matrix[j][i];
}
}

return transposedMatrix;
}

// Transpose the matrix
const transposed = transposeMatrix(matrix);

## What is the difference between .forEach and .map?

.forEach(): It is a method used to iterate over each element in an array and perform a provided callback function on each element. It does not return a new array. The primary use of .forEach() is to perform side effects or operations that do not require a transformed array.
Example using .forEach()

.map(): It is a method used to iterate over each element in an array, apply a provided callback function to each element, and return a new array containing the results of the callback function. The purpose of .map() is to transform an array into a new array based on some transformation logic.

### Objects

## How are objects different from arrays?

Arrays are ordered collections of elements accessed by numerical indices, whereas objects are collections of key-value pairs where each value is associated with a unique key. Arrays are suitable for handling ordered data, while objects are ideal for handling unordered data and modeling real-world entities. Arrays use square brackets for representation, while objects use curly braces. Arrays have built-in iteration methods, while objects can be iterated using for...in loops or object-specific methods like Object.keys().

## What does this keyword do? Explain in detail

1. Global Context:
   When this is used in the global scope (outside of any function or object), it refers to the global object. In a browser environment, the global object is usually window. For example:

console.log(this); // Refers to the global object (e.g., window in a browser)

2. Object Methods:
   When this is used within a method of an object, it refers to the object itself. It allows access to other properties and methods of the object. For example:

const myObject = {
name: "John",
sayHello: function() {
console.log("Hello, " + this.name);
}
};

myObject.sayHello(); // Logs "Hello, John"

3. Function Context:
   The value of this inside a standalone function depends on how the function is called. It can vary based on the execution context. For example:

function greet() {
console.log("Hello, " + this.name);
}

const person = {
name: "Alice"
};

greet(); // Logs "Hello, undefined"

person.greet = greet;
person.greet(); // Logs "Hello, Alice"

4. Constructor Functions:
   When a function is used as a constructor with the new keyword, this refers to the newly created object. The function's prototype is automatically assigned to the new object. For example:

function Person(name) {
this.name = name;
}

const john = new Person("John");
console.log(john.name); // Outputs "John"

## What are the different types of scopes? What are the differences?

Global Scope: Variables declared outside of any function or block have global scope. They are accessible throughout the entire program.

Function Scope: Variables declared within a function have function scope. They are only accessible within the function and any nested functions.

Block Scope: Variables declared with let or const within a block (e.g., inside curly braces {} of an if statement or a for loop) have block scope. They are only accessible within that block.

The differences between these scopes can be summarized as follows:

Global scope is accessible throughout the entire program, while function and block scopes have more limited access.
Function scope variables are accessible within the function they are declared in and any nested functions.
Block scope variables are accessible within the block they are declared in, including nested blocks.
Variables declared with let or const have block scope, while variables declared with var have function scope.

## What are constructors?

Constructors are functions used to create and initialize objects based on a defined blueprint or class. They are invoked with the new keyword to create new instances of the object.

## What is hoisting? How does hoisting work?

Hoisting is a JavaScript behavior where variable and function declarations are moved to the top of their scope during compilation, allowing them to be accessed before they are defined in the code.

## Explain closures?

A closure in JavaScript is a combination of a function and the lexical environment in which it was declared. It allows a function to access variables from its outer scope even after the outer function has finished executing. Closures are useful for creating private variables and functions, encapsulating data, and managing asynchronous operations.
function outer() {
const outerVar = 'Hello';

function inner() {
const innerVar = ' World';
console.log(outerVar + innerVar);
}

return inner;
}

const myFunction = outer();

## What is debouncing? What is throttling? Implement a simple solution on the frontend.

Debouncing and throttling are techniques used in web development to control the frequency of certain events, such as resizing the window or scrolling, to improve performance and optimize resource usage.

Debouncing:
Debouncing is a technique that ensures a function is only executed after a specified period of inactivity. It is typically used to delay the execution of a function until the event triggering it has stopped firing for a certain duration. This is useful when you want to perform an action after the user has finished a series of rapid events.

Throttling:
Throttling is a technique that limits the rate at which a function is executed. It ensures that the function is called at a fixed interval, preventing it from being called more frequently than the specified time interval. Throttling is helpful when you want to limit the frequency of an event to prevent it from being triggered too often.

function debounce(func, delay) {
let timerId;

return function() {
clearTimeout(timerId);
timerId = setTimeout(func, delay);
};
}

// Usage example
function handleScroll() {
console.log('Scroll event debounced');
}

const debouncedScroll = debounce(handleScroll, 300);
window.addEventListener('scroll', debouncedScroll);

<!-- -------------------------------------------------------------------- -->

function throttle(func, delay) {
let timerId;
let isThrottled = false;

return function() {
if (isThrottled) return;

    func();
    isThrottled = true;

    timerId = setTimeout(function() {
      isThrottled = false;
    }, delay);

};
}

// Usage example
function handleResize() {
console.log('Resize event throttled');
}

const throttledResize = throttle(handleResize, 500);
window.addEventListener('resize', throttledResize);

##
