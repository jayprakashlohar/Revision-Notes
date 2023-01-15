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
