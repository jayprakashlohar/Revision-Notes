### Redux

## What is Redux? 

Redux is an open-source JavaScript library for managing application state. It is most commonly used with libraries such as React or Angular for building user interfaces. Redux provides a state container for JavaScript applications that helps manage the state of the application and enforce the unidirectional data flow.

## What are actions in redux?

In Redux, actions are plain JavaScript objects that represent an event that has occurred in the application. Actions are the only way to trigger a state change in the store, and must include a type property that indicates the type of action being performed. Actions are dispatched to the store with the store.dispatch() method, and the data contained within the action is processed by the reducer to update the state of the application.

## What are action creators in redux? 

Action creators are functions that return an action, which is an object that contains a type property and optionally a payload. Action creators are used to make code more readable and maintainable in large Redux applications. They allow for the easy creation of action objects that can be dispatched to the store or middleware for further processing.

## What are dispatchers?

Dispatchers in Redux are functions that send an action to the reducer. They are used to trigger changes in the state of the application by dispatching an action to the store. Dispatchers are the only way to trigger a state change in a Redux application and they must be called within an action creator.

## What are reducers?

Reducers are pure functions that take the current state of an application and an action, and return a new state. They are the most important concept in Redux and are the only thing that can update the state of the application. Reducers are responsible for producing the new state of the application in response to an action.

## What are reducers?

REDUCER: In redux, the reducers are the pure functions that contain the logic and calculation that needed to be performed on the state. These functions accept the initial state of the state being used and the action type. It updates the state and responds with the new state

## What are pure functions?

A Pure Function is a function (a block of code) that always returns the same result if the same arguments are passed. It does not depend on any state or data change during a program’s execution. Rather, it only depends on its input arguments.
Also, a pure function does not produce any observable side effects such as network requests or data mutation, etc.

## Why do we spread the state or return a new object in reducers?

We spread the state or return a new object in reducers to ensure that the state is immutable. This means that the state object should not be changed directly. Instead, a modified copy of the state should be returned. This allows us to keep track of changes to the state and helps maintain the integrity of the data.

## Why do dispatchers take only actions which are objects?

Dispatchers take only actions which are objects because it helps to ensure that the dispatcher is following proper protocols and procedures. Objects can be tracked and documented, which makes it easier for the dispatcher to keep accurate records of all actions taken. This also helps to ensure that the dispatcher is following the law and is not taking any illegal or unethical actions.

## What are types in actions why do we need them?

Types in actions are a way to represent an action that can be taken in an application. They are used to provide a consistent way to refer to and use the same action throughout the application. Types in actions are usually defined as constants so that they can be used in multiple places and can be referenced in the same way throughout the application. Types in actions are important for providing a consistent way to refer to and use actions, which can help make the code more maintainable and easier to debug.

## What happens when you pass a function into a dispatcher?

When you pass a function into a dispatcher, the dispatcher will execute that function. Depending on the type of dispatcher, this may involve passing parameters to it, scheduling the execution of the function, or performing other tasks related to executing the function.

## Where do dispatchers come from?

Dispatchers come from the Redux store. They are functions that can be used to send actions (data) to the store. Generally, dispatchers are contained in a separate file, such as an 'actions' file, and then imported into the store.

## What are the properties of a store?

Store: It is an object which provides the state of the application. This object is accessible with help of the provider in the files of the project. The only way to change the state inside it is to dispatch an action on it.

There are three important parts of the store:
createStore(): To create a store object in redux.
dispatch(action): To change the state of store data by using the actions.
getState(): For getting the current state of the store in redux.

## What is the difference between Context API and Redux?

The main difference between Context API and Redux is that Context API is a built-in React library that allows components to access data without having to pass the data down through multiple levels of components, while Redux is a third-party library that provides a global state management solution. Context API is much easier to implement and more lightweight than Redux, but Redux offers more features, such as time-travel debugging, and is better suited for large-scale applications.

## What are redux thunks?

Redux Thunks are an asynchronous middleware for Redux that allows developers to write action creators that return a function instead of an action. This function, called a thunk, can contain arbitrary logic, including making asynchronous API calls. It is used to delay the dispatch of an action, or to dispatch only if a certain condition is met. This is useful for complex actions such as creating or updating data in a database.

## Why do we need to use network requests in redux thunks?

Network requests in redux thunks allow us to easily dispatch actions that make asynchronous calls to external APIs. This allows us to retrieve data from external sources, like fetching data from a server or making a call to an external API, and use that data in our Redux store. By using network requests in redux thunks, we can easily maintainthinks our application state in an asynchronous manner.

## What are middlewares in redux?

Middlewares in Redux are functions that allow the store to intercept and act upon dispatched actions before they reach the reducer. Middlewares are useful for logging data, performing asynchronous tasks, and dispatching other actions.

## Can you write your own middleware instead of thunks? what do thunks do?

Yes, you can write your own middleware instead of thunks. Thunks are functions that are used to delay the evaluation of an expression. They can be used to perform asynchronous tasks such as data fetching, impure functions such as accessing the browser cache, and other tasks that require some form of deferred execution. Thunks are commonly used in Redux to manage asynchronous actions, allowing us to dispatch asynchronous actions in our reducers and pass the action payloads to the store.

## What is useSelector?

useSelector is a React hook that allows a component to access the data from a Redux store. It allows components to subscribe to the store and be notified of any changes. It is the primary way to access state in a Redux application.

## What is the compareFn that you pass in a useSelector?

The compareFn is a function that is passed into the useSelector hook. It is used to compare the current state to the previous state and determines if the selector needs to be re-run or not. The compareFn takes two parameters, the previous state and the current state, and returns a boolean that indicates whether the selector should be re-run.

## What is useDispatch?

useDispatch is a React hook that is used to dispatch an action to a Redux store. It takes in an action object as an argument and returns a dispatch function that can be used to dispatch the action to the store. This is a powerful way to access the store and update state via Redux.

## What is the use of Provider?

Provider is an abstraction on top of React’s Context API which allows us to pass data through the component tree without having to pass props down manually at every level. It helps to avoid the tedious context passing through many components and makes it easier to share data across components.

## what is redux tool kit? How does it make redux better?

Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code. Redux Toolkit is beneficial to all Redux users regardless of skill level or experience

<!-- ????????? -->

## what is action in redux?

Action in Redux is a plain JavaScript object that represents an intention to change the state of the application. Actions are the only source of information for the store. They are sent to the store using store.dispatch(). Actions must have a type property that indicates the type of action being performed.

## what is reducer in redux?

Reducers in Redux are functions that take in the current state of an application, an action, and return a new state. Reducers are the only source of truth for state in Redux, and they must be pure functions, meaning they must return the same output given the same input. Reducers are responsible for updating the application's state in response to an action.

## what is store in redux?

Redux is a state management library for JavaScript applications. It stores the application's state in a single, immutable object. This allows for the application to have a single source of truth for its state, which makes it easier to debug and maintain.

## 
