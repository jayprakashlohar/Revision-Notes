### NODE JS QUESTIONS

## Explain the difference between local and global npm packages.

Local npm packages are installed in the local project directory and are available only within the current project. They are useful for creating custom packages that are specific to the project. Local packages are installed using the npm install <package> command.

Global npm packages are packages that are installed outside of the current project. They are available across all projects and can be accessed from anywhere on the system. Global packages are installed using the npm install -g <package> command.

## Why does Node.js prefer error-first callback?

Node.js prefers error-first callbacks because it allows for better error handling and allows for the program to have a more consistent flow. The error-first callback also allows developers to easily detect errors as they occur, resulting in programs that are more stable and reliable. Additionally, it makes it easier to debug code, since errors will be identified quicker and more easily.

## Explain Types of hooks in node?

- The following are the different types of hooks in Node.js:

1. Async hooks: These hooks allow you to execute asynchronous code in a non-blocking way.
2. Timers: These hooks enable you to schedule code execution at a specified time.
3. Error hooks: These hooks allow you to catch errors and take appropriate actions.
4. Process hooks: These hooks allow you to monitor the events in the process lifecycle.
5. I/O hooks: These hooks enable you to perform input and output operations.
6. Domain hooks: These hooks enable you to manage multiple related operations as a single unit.
7. Console hooks: These hooks allow you to log messages to the console.

## What are benefits of node js?

1. Fast: Node.js is built on Google Chrome’s V8 JavaScript engine, which makes it very fast.

2. Scalable: Node.js is highly scalable, as it is built on a single-threaded, non-blocking model. This makes it very efficient in handling multiple concurrent requests without creating additional threads.

3. Asynchronous and Event-Driven: All API's of Node.js library are asynchronous and being event-driven, which makes it a very fast and efficient runtime environment.

4. No Buffering: Node.js applications never buffer any data, as it outputs the data in chunks.

5. Easy to learn: Node.js is an open source platform and has an extensive and vibrant community of developers who are always willing to help newbies.

6. Easy to deploy: Node.js applications can be deployed quickly and easily.

7. Modular and Reusable Code: Node.js allows developers to reuse code and create modules that can be shared with the development community.

## Explain Git commands?

Git is a version control system that keeps track of changes in source code over time. It helps developers collaborate on projects more easily by allowing them to work on the same codebase without disrupting each other's work.

1. git init: This command is used to initialize a new Git repository.
2. git add: This command is used to add files to the staging area.
3. git commit: This command is used to commit changes to the repository.
4. git push: This command is used to push changes to a remote repository.
5. git pull: This command is used to pull changes from a remote repository.
6. git branch: This command is used to create, list, or delete branches in the repository.
7. git merge: This command is used to merge branches in the repository.
8. git status: This command is used to check the status of the repository.
9. git checkout: This command is used to switch between branches in the repository.
10. git log: This command is used to view the commit logs of the repository.

## How do you find a node developer if you are a hiring manager?

1. Post a job listing on job boards and professional networks such as Indeed, LinkedIn, AngelList, and Stack Overflow.
2. Reach out to relevant communities and user groups on social media and forums like Reddit, GitHub, and Stack Exchange.
3. Connect with experienced node developers on LinkedIn and other professional networks.
4. Ask colleagues and peers for referrals.
5. Utilize recruitment agencies that specialize in finding node developers.
6. Run targeted advertisements on job boards and social media.

## Lifecycle methods of nodejs?

1. init() – This method is used to initialize the application.
2. start() – This method is used to start the application.
3. stop() – This method is used to stop the application.
4. shutdown() – This method is used to shutdown the application.
5. reload() – This method is used to reload the application.
6. restart() – This method is used to restart the application.
7. on(event, listener) – This method is used to register an event listener.
8. removeListener(event, listener) – This method is used to remove an event listener.

## Data validation and data verification in node?

Data validation is the process of ensuring that the data that is entered into a system is accurate and valid. It is used to ensure that data conforms to the rules or standards defined by the application or system. Data validation can be done through a variety of methods, including client-side scripting, server-side scripting, or manual review of the data.

Data verification is a process of ensuring that the data that is stored in the system is correct and has not been altered in any way. This is usually done by comparing the data with a known source, such as a checksum or hash. Data verification can also be done manually by comparing the data against a set of rules or standards.

### REACT JS QUESTIONS

## What is React? Why do we use React?

React is a JavaScript library used for building user interfaces. It is component-based, which allows developers to break down complex user interfaces into small, reusable components that can be managed more easily. React is used by many developers because of its declarative syntax which makes the code more readable, maintainable, and testable. Additionally, React allows developers to create highly interactive UIs, which is ideal for single page applications.

## Create a react app where count should start adding on the page

load and on stop button click, count should stop adding?

import React, { useState, useEffect } from 'react';

function App() {
const [count, setCount] = useState(0);
const [isRunning, setIsRunning] = useState(false);

useEffect(() => {
let interval;
if (isRunning) {
interval = setInterval(() => setCount(count + 1), 1000);
}
return () => {
clearInterval(interval);
};
}, [isRunning, count]);

return (

<div>
<h1>{count}</h1>
<button onClick={() => setIsRunning(!isRunning)}>
{isRunning ? 'Stop' : 'Start'}
</button>
</div>
);
}

export default App;

## What is useState?

useState is a Hook that allows you to add React state to function components. It takes a single argument, which is the initial state, and returns an array with two values: the current state and a function that updates it.

## What is useEffect?

UseEffect is a React hook that allows you to perform side effects in function components. It is a combination of componentDidMount, componentDidUpdate, and componentWillUnmount lifecycle methods. With useEffect, you can perform any type of side effect, such as data fetching, setting up a subscription, and manually changing the DOM.


## 