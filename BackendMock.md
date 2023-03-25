## Backend

## What is the difference between readFile and readFileSync.

The main difference between readFile and readFileSync is that readFile is asynchronous and readFileSync is synchronous. Asynchronous functions are non-blocking, meaning that other code can be executed while the asynchronous function is running. Synchronous functions are blocking, meaning that the next line of code will not be executed until the synchronous function has finished running.

## How to create a web server without express? Write some basic Routes.

There are several ways to create a web server without Express.
The most basic way is to use the built-in Node.js http module.
Below is a simple example of a web server using the http module:
const http = require('http');

const hostname = '127.0.0.1';
const port = 3000;

const server = http.createServer(function(req, res) {
res.statusCode = 200;
res.setHeader('Content-Type', 'text/plain');
res.end('Hello World\n');
});

server.listen(port, hostname, function() {
console.log(`Server running at http://${hostname}:${port}/`);
});

The following is an example of basic routes for the above web server:

// Home page route
app.get('/', (req, res) => {
res.status(200).send('Welcome to the home page');
});

// About page route
app.get('/about', (req, res) => {
res.status(200).send('Welcome to the about page');
});

// Contact page route
app.get('/contact', (req, res) => {
res.status(200).send('Welcome to the contact page');
});

## What is the difference between common JS and EJS module?

CommonJS is a JavaScript module system that is used in most JavaScript engines. It is used to define dependencies between modules, which can be loaded synchronously or asynchronously. It is used in server-side applications and in Node.js.

EJS (Embedded JavaScript) is a templating language that allows developers to write HTML with JavaScript code. It simplifies development by separating the logic from the HTML markup. It is used mainly in web development and is often used in combination with Node.js. Unlike CommonJS, EJS does not support module dependencies or asynchronous loading.

## What is JWT and what we can achieve with that?

JWT (JSON Web Token) is an open standard for securely transmitting information between parties as a JSON object. It is commonly used to authenticate users and provide access to protected resources, such as APIs. JWTs are signed using a secret key or a public/private key pair and can be used to authenticate users, verify the integrity of data, and ensure the non-repudiation of requests. Additionally, JWTs can be used to securely share data between applications, reducing the need for API calls and enabling faster communication.

## What should we do with the password of a user before storing it into DB?

We should always hash the user's password before storing it into a database. Hashing is a one-way encryption technique that takes a plaintext password and converts it into a unique, unrecognizable string of characters (called a "hash"). This makes it much harder for a malicious actor to gain access to the user's account, as the original password cannot be recovered from the hash.

## What is File stream?

File stream is a feature of Google Drive that allows users to store and access their files from anywhere. It is designed to handle large files that are too large to store in the cloud. File stream allows users to securely sync and access their files from any device. It also provides fast, reliable access to files, even when the user is offline.

## What are middlewares, and how they can help us?

Middlewares are software components that enable applications to interact with other applications and systems. They act as an intermediary between two endpoints, allowing data to be sent, received, and processed. Middlewares can help us by providing a bridge between different systems and applications, enabling data to be transmitted securely and quickly, and allowing us to develop more complex applications. Additionally, middlewares can help optimize application performance, provide security, handle errors, and manage transaction

## How can we take inputs from terminal?

We can take inputs from the terminal using the following methods:

1. Using the `input()` function: This function takes a single argument which is a string that is printed to the terminal. It then waits for the user to enter a response, and returns the inputted string.

2. Using the `raw_input()` function (Python 2 only): This function works similarly to the `input()` function, but it allows the user to enter multiple lines of input.

3. Using the `sys.stdin.readline()` function: This function reads a single line of input from the terminal. The line is returned as a string.

4. Using the `sys.stdin.readlines()` function: This function reads multiple lines of input from the terminal. The lines are returned as a list of strings.

## How many types of modules are there in node?

There are three main types of modules in Node.js: Core Modules, Local Modules, and Third-Party Modules. Core Modules are modules that are included in the Node.js installation and provide basic functionalities. Local Modules are modules that are created by the user in the application’s directory and are used by the application. Third-Party Modules are modules that are created by other developers and are installed using the Node Package Manager (NPM).

## What is the difference between authentication and authorization?

Authentication is the process of verifying that someone is who they claim to be, while authorization is the process of verifying that someone has the right to access or perform a certain action. Authentication is used to identify users, while authorization is used to grant access to resources.

Authentication and authorization are two vital information security processes that administrators use to protect systems and information. Authentication verifies the identity of a user or service, and authorization determines their access rights. Although the two terms sound alike, they play separate but equally essential roles in securing applications and data. Understanding the difference is crucial. Combined, they determine the security of a system. You cannot have a secure solution unless you have configured both authentication and authorization correctly.
