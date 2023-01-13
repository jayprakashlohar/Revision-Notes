### React

## what is react ?
# React is a JavaScript library for building user interfaces.
React is a JavaScript library created by Facebook
React is a User Interface (UI) library
React is a tool for building UI components#

## What are keys in React?

* A “key” is a special string attribute you need to include when creating lists of elements in React. Keys are used in React to identify which items in the list are changed, updated, or deleted. In other words, we can say that keys are used to give an identity to the elements in the lists*

## What is memoisation in react?

* Memoization is an optimization technique for accelerating computer programs by caching the results of heavy function calls and returning them when similar inputs are encountered repeatedly. Simply, React memoization is similar to caching.*

## What is the difference between react.memo and react.useMemo?

* The major difference between React.
React. memo is a higher-order component to memoize an entire functional component. useMemo is a react hook to memoize a function within a functional component*

## How does Routing work with react?

* React Router is a standard library for routing in React. It enables the navigation among views of various components in a React Application, allows changing the browser URL, and keeps the UI in sync with the URL.
Let us create a simple application to React to understand how the React Router works. The application will contain three components: home component, about a component, and contact component. We will use React Router to navigate between these components.*

## What is SSR and CSR?

* The main difference between CSR and SSR is where the page is rendered. SSR renders the page on the server-side and CSR renders the page on the client-side. The client-side dynamically manages the routing without refreshing the page each time the client requests another route.*

## What are the lifecycle methods in class components?

**What are dependencies in useEffect?

* useEffect(callback, dependencies) is the hook that manages the side-effects in functional components. callback argument is a function to put the side-effect logic. dependencies is a list of dependencies of your side-effect: being props or state values.*

## What is a pure component?

* A React component is considered pure if it renders the same output for the same state and props.
Generally, In ReactJS, we use shouldComponentUpdate() Lifecycle method to customize the default behavior and implement it when the React component should re-render or update itself.
*

## What is useCallback?

* useCallback is a hook that will return a memoized version of the callback function that only changes if one of the dependencies has changed. Memoization is a way to cache a result so that it doesn't need to be computed again. This can boost performance*

## What are callback refs?

* The function receives the React component instance or HTML DOM element as its argument, which can be stored and accessed elsewhere.*

## How does Context API work? What does it solve?

* The Context API helps share data between components which you can't easily share with props, for example, complex data objects. React Context API provides a way to send data like userid, auth, and theme data through the component tree without sending any props manually at every level. *

## What does useReducer do?

useReducer is a React hook that allows you to manage state in a function component. It is used for a more complex state management than useState, and is an alternative to Redux. It takes two arguments: a reducer function and an initial state, and it returns the current state, and a dispatch function to update the state.

## When do you use useReducer vs useState?

UseReducer is typically used for more complex state management, such as when you need to manage state when there are multiple actions and mutations. It can also be helpful when you need to access previous state values within a reducer. On the other hand, useState is more suitable for simple state management, such as toggling a boolean or setting a string value.

## How do you use Profiler?

Profiler is a software application that can be used to assess the performance and security of a system. It can be used to identify bottlenecks, measure resource utilization, detect malware and malicious code, and provide insights into application behavior. To use Profiler, you first need to create a profile of your system, which is a set of parameters that define how the software will interact with the system. Once the profile is created, you can then run the Profiler to analyze the system and generate reports. These reports can then be used to make informed decisions on how to optimize system performance and security.

## What is dispatcher in react?
The dispatcher is the center point of the data flow in a Flux application. It is simply a directory of call-backs and incites these callbacks in a particular order. Callbacks are stored in each and every store with a dispatcher.

## What is flux architecture?
Flux architecture is an application architecture developed by Facebook for building user interfaces. It is based on a unidirectional data flow and follows an event-driven approach. Flux architecture is composed of four main components: the dispatcher, the stores, the views, and the actions. The dispatcher is responsible for dispatching events to the stores and views, the stores are responsible for managing application state, the views are responsible for responding to user interactions and emitting events, and the actions are responsible for creating events.

## 