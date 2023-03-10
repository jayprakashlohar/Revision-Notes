## What is the difference between .call() .apply() and .bind()? explain with an example

.call() and .apply() are both methods used to invoke a function with a given this value and arguments provided individually. The difference between them is that .call() takes arguments as individual parameters while .apply() takes arguments as an array. 

For example,

function greet(greeting, name) {
  console.log(`${greeting}, ${name}`);
}
greet.call(null, 'Hello', 'John'); // Output: Hello, John
greet.apply(null, ['Hello', 'John']); // Output: Hello, John
.bind() is also used to invoke a function with a given this value but it will only partialy apply the arguments and return a new function to be invoked later.
For example,
function greet(greeting, name) {
  console.log(`${greeting}, ${name}`);
}
const sayHello = greet.bind(null, 'Hello');
sayHello('John'); // Output: Hello, John

##  Explain Event bubbling and Event Capturing in JavaScript with suitable examples

Event bubbling is the process of an event propagating from the innermost element to the outermost element in the DOM tree. When an event is triggered on a child element it bubbles up and triggers the same event on all parent elements.

For example, if you have a <div> element inside a <form> element and you click on the <div> element, the click event will trigger on the <div> element first and then bubble up to the <form> element.

Event capturing is the opposite of event bubbling. It is the process of an event propagating from the outermost element to the innermost element in the DOM tree. When an event is triggered on a parent element it is captured by the parent and then propagated to all its child elements.

For example, if you have a <form> element containing a <div> element and you click on the <form> element, the click event will trigger on the <form> element first and then be captured by the <div> element.

## What is function currying with example?

Function currying is the process of breaking down a function into a series of functions that each take a single argument. For example, let's say we have a function that adds three numbers: 

const addThree = (a, b, c) => a + b + c; 

We can use currying to break this down into three separate functions, each of which takes one argument: 

const addOne = a => b => c => a + b + c; 
 
const addTwo = b => c => a => a + b + c;

const addThree = c => a => b => a + b + c;

## What is the difference between real DOM and virtual DOM?

Real DOM is a representation of the HTML document structure, which is very slow when it comes to manipulating the HTML elements. It updates the whole HTML tree structure whenever a single element changes, which makes it inefficient for large websites.

Virtual DOM, on the other hand, is a virtual representation of the HTML document structure. It uses JavaScript to create a lightweight copy of the HTML tree structure and then updates the copy whenever an element changes. This process is much faster than the real DOM and it does not affect the actual HTML document structure.

## Why did you choose React over other Libraries and Frameworks?

I chose React because of its flexibility and scalability. It is component-based and makes it easy to create maintainable and reusable code. Additionally, React has a large, active community and a great ecosystem of libraries and tools to support developers. React also allows for faster development and has great performance. Lastly, it is very easy to learn and use.

## What is prop drilling and explain it with an example (parent to child)

Prop drilling, also known as “prop-passing” or “prop-bubbling”, is the process of passing props from a parent component to a child component. It is commonly used when a parent component contains data or methods that need to be accessed by a child component.

For example, if a parent component contains an array of data, it would need to pass that data to a child component so that it can use it. This can be done using prop drilling. The parent component would pass the array of data to the child component as a prop, which the child component can then access and use.

## What is the difference between function and class components?

Function components are a way of writing React components using a plain JavaScript function. They are typically used for components that don’t need to maintain any internal state or use lifecycle methods.

Class components are ES6 classes that extend the React.Component class. They are typically used for components that need to maintain internal state, use lifecycle methods, or need access to React's context.

## Explain the lifecycle method of React Components.

The lifecycle methods of React components are methods that get called automatically at different points when a component is created and destroyed. 

The component lifecycle consists of four distinct phases:

1. Initialization: This is the first phase of a React component lifecycle, where the component is initialized with default props and state. In this phase, the componentWillMount() lifecycle method is called, followed by the render() method, and then the componentDidMount() method. 

2. State/Property Updates: This is the second phase of the React component lifecycle, where the component's state and properties are updated. In this phase, the componentWillReceiveProps() and shouldComponentUpdate() lifecycle methods are called, followed by the render() method, and then the componentDidUpdate() method.

3. Unmounting: This is the third phase of the React component lifecycle, where the component is unmounted from the DOM. In this phase, the componentWillUnmount() lifecycle method is called.

4. Error Handling: This is the fourth phase of the React component lifecycle, where any errors that occur during rendering, mounting, or updating are handled. In this phase, the

## Explain the Flow of Redux.

Redux is a predictable state management library for JavaScript applications. The core idea behind Redux is that the entire application state is stored in a single state tree, which is a plain JavaScript object. This state tree is read-only and can only be changed by dispatching an action.

1. The application dispatches an action: An action is a plain JavaScript object that describes what happened in the application.

2. The reducer: The reducer is a pure function that takes the current state tree and the action being dispatched as arguments and returns the new state tree. It is responsible for updating the state tree in response to actions being dispatched.

3. The store: The store is an object that holds the current state tree of the application and allows access to the state via getState(). It also allows the application to dispatch actions and register listeners via subscribe().

4. The view: The view is the portion of the application that the user interacts with. It is typically a React component. When the state is updated, the view will be re-rendered with the new state.

## What are hooks? Explain a few hooks you have used.

Hooks are a feature of React that allow developers to access state and other features of the React library without having to write a class component. Hooks allow developers to write functional components, which are simpler and more performant than class components.

I have used the useState hook, which allows developers to store and update state in a functional component. I have also used the useEffect hook, which allows developers to run code after a component has rendered. Finally, I have used the useContext hook, which allows developers to access the React context from within a functional component.

Hooks are a feature of React that allow developers to access state and other features of the React library 
without having to write a class components. Hooks allow developers to write. It us typically a React '
component. 