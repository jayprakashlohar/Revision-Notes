## What are closures with examples?

A closure is a function that remembers and accesses its lexical scope even when the function is executing outside its lexical scope. Closures are created every time a function is created and can access variables from their parent scope.

Example:

function greet(name) {
let message = `Hello ${name}!`;

// This inner function has access to the variable message defined in the parent scope
return function() {
console.log(message);
}
}

// Here we create a new closure
let closure = greet('John');

## What is meant by higher-order function?

A higher-order function is a function that takes one or more functions as arguments, or returns a function as a result. It is a function that operates on other functions, either by taking them as arguments or by returning them. Examples of higher-order functions include map, reduce, filter, and compose.

## Difference between Var Let and const?

Var: Variables declared with the 'var' keyword can be reassigned and redeclared within their scope.
Let: Variables declared with the 'let' keyword can be reassigned but can not be redeclared within their scope.
Const: Variables declared with the 'const' keyword can neither be reassigned nor redeclared within their scope.

## What is call, apply and bind?

Call, apply, and bind are all methods of invoking functions in JavaScript. Call is used to invoke a function with individual arguments, while apply is used to invoke a function with an array of arguments. Bind is used to create a new function with the same body and scope as the original function, but with some arguments already fixed.

## What are the differences between call, apply and bind?

Call and apply are methods used to invoke a function with an explicit this context and arguments. The difference between them is in the way the arguments are passed.
Call takes in arguments one by one, while apply takes in an array of arguments.
Bind is similar to call, but instead of invoking the function, it creates a new function with the same context and arguments.

## Difference between map and ForEach?

Map:
Map creates a new array with the results of calling a provided function on every element in the calling array.

ForEach:
ForEach executes a provided function once for each array element. It does not create a new array.

## What is Hoisting?

Hoisting is the JavaScript mechanism where variables and function declarations are moved to the top of their scope before code execution. This means that no matter where functions and variables are declared, they are moved to the top of their scope regardless of whether their scope is global or local. This behavior is called “hoisting” in JavaScript.

## What are hooks?

Hooks are special functions that let you “hook into” React state and lifecycle features from function components. Hooks don’t work inside classes — they let you use React without classes. Hooks allow you to use features like state, lifecycle, context, and more without having to write a class.

## What are useEffect and useRef?

useEffect is a React hook that allows you to perform side effects in function components. It is a combination of componentDidMount, componentDidUpdate, and componentWillUnmount lifecycle methods. It can be used for data fetching, setting up subscriptions, and manually changing the DOM in React components.

useRef is a hook that provides a mutable object of the same type. It can be used to store mutable values across renderings such as a DOM element, function, or object. It can also be used to create references to the DOM elements in order to access methods or properties on those elements.

## What is the difference between useState and useEffect?

The useState hook allows you to manage and update state in a functional component. It is used to set the initial state of a component and to update the state when an event occurs.

The useEffect hook is used for side effects such as data fetching, manually changing the DOM, and subscribing to events. It runs after every render and can be used to perform tasks that are related to the component's state, such as fetching data or setting up subscriptions. It is also used to perform clean-up logic when the component unmounts.

## What is a rest operator?

The rest operator (also known as the spread operator) is a special syntax used in JavaScript to allow an expression to accept multiple arguments or an array of elements. The rest operator allows you to write functions that take a variable number of arguments. It is denoted by three dots (...) followed by the name of the array. The rest operator allows you to pass an indefinite number of arguments to a function as an array.

## What is the spread operator?

The spread operator is a feature of JavaScript that allows an expression to be expanded in places where multiple arguments (for function calls) or multiple elements (for array literals) are expected. It is denoted by an ellipsis (...). The spread operator can be used to spread the contents of an array into a list of arguments or elements. It can also be used to merge two arrays or objects together.

## What is Memoization?

Memoization is a technique used in computer programming to help speed up the execution of certain algorithms by storing the results of expensive function calls and returning the cached result when the same inputs occur again. It is commonly used in dynamic programming algorithms to avoid recomputing the same results, and in functional programming for caching results of expensive computations.

## What is Redux?

Redux is a JavaScript library for managing application state. It is mostly used with React and other view libraries, and is an implementation of the Flux architecture for managing data flow in client-side applications. Redux provides a way to effectively manage and control the state of your application, with a single source of truth for all of your data. It is also used for server-side rendering, in which data can be stored on the server, as opposed to the client.

## Difference between shallow copy and deep copy.

Shallow copy is a bit-wise copy of an object, which means that any changes made to a copy of the object will affect the original object. Deep copy is a recursive copy of all of the objects properties, which means that any changes made to a copy of the object will not affect the original object.

## What will be the output of [] === []? why

The output is false because two empty arrays are not the same object. JavaScript uses a strict comparison operator (===) which means both the value and the type must be the same for the expression to be true.

## What is the difference between FrameWork and Library?

A framework is a collection of libraries and other components that provide a structure for the development of applications. A library is a collection of code that can be used by different applications or programs without having to rewrite the code. A framework provides a specific structure, while a library is a reusable piece of code that can be used in multiple applications.

## What are callback functions?

Callback functions are functions that are passed as an argument to another function and are executed after the outer function has completed its execution. They allow for the execution of a certain task after the completion of some other task. They are also known as higher-order functions because they accept other functions as arguments.

## What do you mean by JSX?

JSX is an XML-like syntax extension to ECMAScript without any defined semantics. It is used by React and other libraries for building user interfaces. It is a syntax that allows developers to write HTML elements and components in the same file as the JavaScript code. JSX allows developers to write HTML code that looks like HTML but also contains JavaScript code that is executed on the client side.

## Explain the flow of redux.

Redux is a state management library that is used to manage the state of an application.

1. The application dispatches an action.

2. The action is picked up by the reducer.

3. The reducer processes the action and returns a new state.

4. The new state is stored in the store.

5. The store notifies the components that the state has changed.

6. The components update and render the new state.

## Create a timer on the codeSandbox.

code in react js

import React, { useState } from "react";

function Timer() {
const [seconds, setSeconds] = useState(0);
const [minutes, setMinutes] = useState(0);

const startTimer = () => {
setInterval(() => {
setSeconds(seconds => seconds + 1);
if (seconds >= 59) {
setMinutes(minutes => minutes + 1);
setSeconds(0);
}
}, 1000);
};

const resetTimer = () => {
setSeconds(0);
setMinutes(0);
};

return (

<div>
<h1>{minutes}:{seconds}</h1>
<button onClick={startTimer}>Start Timer</button>
<button onClick={resetTimer}>Reset Timer</button>
</div>
);
}

export default Timer;

## How does React work?

React is a JavaScript library for building user interfaces. It works by breaking down a user interface into components, which are small, reusable pieces of code. These components are then rendered in the browser, with data being passed between the components. React also has features such as a virtual DOM, which keeps track of changes to the DOM and only updates the parts that need to be updated. This helps to make React apps more efficient and perform better.

## Difference between React and Redux.

React is a JavaScript library for building user interfaces, while Redux is a state management library used to build complex applications. React focuses on rendering data to the DOM, while Redux is used to manage the data in the application. React is used to create a view, while Redux is used to manage the state of the application. React is just a library, while Redux is a combination of libraries, technologies, and principles.

## What is the difference between redux and context API?

Redux is a global state management library, while the Context API is a built-in React feature for managing state locally in a component tree. Redux is more complex and requires more setup, while the Context API is easier to use and requires less code. Redux is better suited for applications with complex state, while Context API is better suited for managing smaller, localized state.

## Explain Async Await?

Async/Await is a set of keywords used in JavaScript to write asynchronous code. It makes writing asynchronous code look like writing synchronous code by using the keywords async and await. Async functions return a Promise, so you can use the await keyword in the function body to pause the function execution until the Promise is settled. The await keyword can only be used inside an async function.

## What is Node Js?

Node.js is an open-source, cross-platform, JavaScript runtime environment that executes JavaScript code outside of a browser. Node.js lets developers use JavaScript to write command line tools and for server-side scripting—running scripts server-side to produce dynamic web page content before the page is sent to the user's web browser. Node.js is available for free for Windows, Linux, and macOS.

## What are Promises and its states?

Promises are objects that represent the eventual completion (or failure) of an asynchronous operation and its resulting value. Promises have three states: pending, fulfilled, and rejected. Pending means that the operation has not yet been completed. Fulfilled means that the operation has been completed successfully. Rejected means that the operation has failed.

## Write a code to generate a Random Number.

import React, { useState } from "react";

function RandomNumberGenerator() {
const [randomNumber, setRandomNumber] = useState(null);

function generateRandomNumber() {
const randomNum = Math.floor(Math.random() \* 100) + 1;
setRandomNumber(randomNum);
}

return (

<div>
<button onClick={generateRandomNumber}>Generate Random Number</button>
{randomNumber && <p>Random Number: {randomNumber}</p>}
</div>
);
}

export default RandomNumberGenerator;

## Difference between states and props.

States and props are both used to keep track of data within a React component. The main difference between them is where the data come from. States are mutable and managed within the component, while props are immutable and passed down from the parent component.

States are used to store data that is local to the component and can be changed over time. This data is accessible and used within the component itself.

Props are used to pass down data from one component to another. They are immutable and cannot be changed by the component. Props are typically passed down from the parent component to the child component.

## What is React fiber?

React Fiber is an ongoing reimplementation of React's core algorithm. It is the first major update to the framework since React was released by Facebook in 2013. Fiber aims to increase its suitability for complex applications by better leveraging asynchronous rendering and by providing a more predictable computational model for building UIs. React Fiber also provides improved performance and improved support for incremental rendering.

## What is middleware? explain with an example.

Middleware is software that acts as a bridge between an operating system and applications, or between two applications. It is designed to facilitate communication and data exchange between two or more systems. For example, a web application might use middleware to facilitate communication between the web server and a database. Middleware would allow the web application to query the database and display the results on the web page in a format that is easy to understand.

## optimization techniques in React.

1. Use React.memo() and React.PureComponent: React.memo() is a higher order component that helps to optimize the performance of functional components and React.PureComponent is a regular component that helps to optimize the performance of class components.

2. Use the React.lazy() and Suspense API: React.lazy() is used to lazily load components and Suspense is used to render a fallback state while the components are loading. This is helpful in scenarios when the user has to wait for the components to load.

3. Use the React.Fragment API: React.Fragment is a special type of component that allows us to return multiple elements without using any extra HTML element. This is helpful in scenarios where we want to render multiple elements but don’t want to add any extra HTML element.

4. Use the React.Profiler API: React.Profiler is a great API that helps to measure the performance of React components. It allows us to track the performance metrics of the application such as the render time, commit time, and more.

5. Use the useCallback() and useMemo() hooks: useCallback() and useMemo() hooks help

## Is React a library?

Yes, React is a JavaScript library for building user interfaces. It is maintained by Facebook and a community of individual developers and companies.

## What is an Event loop?

An event loop is an asynchronous programming construct that allows an application or program to continually listen for and respond to events or messages from other programs. It is the core of any event-driven programming, and allows for a program to run indefinitely and continuously respond to outside events.

## What is an Event loop?

An event loop is an asynchronous programming construct that allows an application or program to continually listen for and respond to events or messages from other programs. It is the core of any event-driven programming and allows for a program to run indefinitely and continuously respond to outside events.

##
