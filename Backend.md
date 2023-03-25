### Backend Genral

## What is Authentication ?

Authentication is the process of verifying the identity of a user or process. This is typically done by validating a username and password combination, but may also involve using biometric data, security tokens, or other methods. Authentication is an important part of computer and network security, as it ensures that only authorized users can access data and resources.

## What is Authorization?

Authorization is the process of granting access to a user or program for certain data or functionality. It involves verifying that a user has the necessary permissions to access a resource, and determining what actions they are allowed to perform on the resource. Authorization typically occurs after a user has successfully authenticated to a system.

## How do you do role-based authentication?

Role-based authentication typically involves the use of an authentication system that requires users to be assigned specific roles, usually based on their job functions. Each role is then assigned different levels of access to resources, depending on the privileges associated with that role. When users attempt to access resources, the authentication system checks their role and grants or denies access accordingly. Common examples of role-based authentication include using Active Directory or LDAP for Windows-based authentication or using a third-party identity provider such as Okta or Auth0 for authentication in web applications.

## What is hashing?

Hashing is a process used to convert data of any size or type into a fixed-length value or key. This key is usually referred to as the hash or message digest. Hashing is used to index and retrieve items in a database, and is also used to provide data integrity. Hashing is a one-way process and cannot be reversed, meaning that the data cannot be reconstructed from the hash.

## What is encryption?

Encryption is the process of encoding information or data in such a way that only authorized parties can access it. It uses complex algorithms and encryption keys to protect data from unauthorized access, modification, or destruction. Encryption is commonly used to protect data in transit, such as when it is sent over the internet, and to protect data at rest, such as when it is stored on a hard drive.

## How is hashing and encryption different?

Hashing is a one-way process that takes an input of any length and produces a fixed-length output. It is used to verify the integrity of data by comparing the hash of the original data with the hash of the data that has been received.

Encryption is a two-way process that takes an input of any length and produces an output of the same length. It is used to protect data by making it unreadable without a key. The key is used to decrypt the data back to its original form.

## What is JWT?

JWT (JSON Web Token) is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWT is typically used to pass authentication and authorization information, such as a user's identity or access rights.

## How is JWT different and list the pros and cons of using JWT tokens?

JWT (JSON Web Token) is a type of authentication token used to authenticate a user on an application. It is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. 

Pros:
- Compact and secure: JWTs are usually smaller in size than other authentication tokens, making them more secure and easier to transmit.
- Verifiable: JWTs can be easily verified using a secret key or a public key.
- Scalable: JWTs can be used across multiple applications and services, making them extremely scalable.

Cons:
- Security: JWTs are not encrypted, which means that any data encoded in them can be accessed by anyone.
- Stateless: JWTs are stateless, meaning that there is no way to track a user’s session.
- Expired tokens: JWTs may expire, making them unreliable for long-term authentication.

## What are the different ways to manage authentication?

1. Password-Based Authentication: This is the simplest form of authentication, where users are required to enter a username and password to gain access to a system.

2. Multi-Factor Authentication (MFA): This type of authentication requires users to provide two or more pieces of evidence to prove their identity. This could include a combination of a password, biometric data, or a security token.

3. Single Sign-On (SSO): This authentication method allows users to access multiple applications with a single set of credentials.

4. Biometric Authentication: This type of authentication uses physical characteristics to verify a user’s identity, such as fingerprints, facial recognition, or voice recognition.

5. Identity Access Management (IAM): This authentication method goes beyond passwords and requires users to provide multiple forms of verification to gain access to a system. It can also be used to control user access to applications and resources.

6. Token-Based Authentication: This type of authentication uses a secure token (such as an OTP) that is sent to a user’s device to verify their identity.

## What is cookie-based auth?

Cookie-based authentication is a method of authenticating users of a website or web application. It works by sending a small piece of data, known as a cookie, to the user's web browser. This cookie contains a unique identifier, which is used to identify the user when they return to the site. The web application can then use this identifier to retrieve the user's information from a database and authenticate them.

## What is session management?

Session management is the process of managing user sessions in a computer or web application. It typically involves tracking the state of a user’s interaction with a web application over multiple requests and providing the user with a consistent experience. Session management typically involves the storage of user data, authentication of users, and the tracking of user activities.

## What is REST api?

REST (Representational State Transfer) is an architectural style for building web services. It is based on a client-server model, where the server is an HTTP-based web service and the client sends and receives data in the form of JSON or XML. REST APIs allow developers to access and manipulate data from a remote server using HTTP requests. They are often used to build web services for mobile and web applications.

## What is a stateless backend?

A stateless backend is an application architecture that does not store any data on the server. It is based on a client/server model, where each client request is handled independently and the server does not store any state information from previous requests. This type of architecture is typically used for web applications and APIs, as it allows for scalability and flexibility.

## What is GraphQL? 

GraphQL is an open-source data query and manipulation language for APIs, developed and used by Facebook. It provides an alternative to REST and ad-hoc web service architectures. GraphQL allows developers to request data from a single endpoint and receive predictable responses. It also allows for better data fetching and manipulation capabilities, allowing developers to ask for the exact data they need, reducing the amount of data sent to and from the server.

## What is gRPC?

gRPC (gRPC Remote Procedure Calls) is an open-source remote procedure call (RPC) system initially developed by Google in 2015. It uses an efficient binary protocol based on HTTP

## What is the client server model?

The client–server model is a distributed application structure that partitions tasks or workloads between the providers of a resource or service, called servers, and service requesters, called clients. Often clients and servers communicate over a computer network on separate hardware, but both client and server may reside in the same system. A server host runs one or more server programs which share their resources with clients. A client does not share any of its resources but requests a server's content or service functions. Clients therefore initiate communication sessions with servers which await incoming requests.

## What is HTTP vs HTTPS?

HTTP (Hypertext Transfer Protocol) is the protocol used for transferring data between a web browser and web server. It is used for transferring web page requests and responses. 

HTTPS (Hypertext Transfer Protocol Secure) is an extension of HTTP that provides an additional layer of security by using encryption. This encryption helps protect information sent between the browser and web server, ensuring that data remains private and secure.

## What is throughput?

Throughput is the measure of how much data is transmitted from one point to another in a given period of time. It is typically measured in bits per second (bps), kilobits per second (Kbps), megabits per second (Mbps) or gigabits per second (Gbps).

## What is availability?

Availability is the percentage of time a system, service, or resource is operational and accessible to users. It is usually expressed as a number between 0 and 1, or as a percentage. High availability is a key component of any reliable system, as it ensures that users have access to the services they require when they need them.

## What is latency?

Latency is the amount of time it takes for a packet of data to travel from one point to another. Latency is measured in milliseconds, and is affected by factors such as the distance between the two points, the type of network connection, and the amount of traffic on the network.

## What is Caching?

Caching is a technology that stores web data such as HTML pages, images, and other files in a temporary storage location so that they can be quickly retrieved and served up to a user. Caching improves the user experience by allowing web pages to load faster and reducing the amount of time and bandwidth it takes to access a web page.

## What are ways to cache on the backend?

1. Content Delivery Networks (CDN): A content delivery network (CDN) is a system of distributed servers that deliver web content to a user based on the geographic locations of the user, the origin of the web page, and the content delivery server.

2. Database Caching: Database caching is a technique that involves storing a copy of frequently-accessed data in memory for quick retrieval. This reduces the amount of time required to access the data from the database.

3. Object Caching: Object caching is a technique for storing frequently-used objects in memory for faster access. The most common type of object caching is web page caching, which stores web pages in memory for faster loading times.

4. In-Memory Caching: In-memory caching is a technique for storing frequently-used data in memory for faster access. In-memory caching is commonly used in applications that require quick access to data, such as web applications.

5. Disk Caching: Disk caching is a technique that involves storing data on a local hard drive for quick retrieval. Disk caching is commonly used in applications that require quick access to data, such as web applications.

## What is LRU cache?

LRU (Least Recently Used) cache is a type of cache memory that is designed to store the most recently used items in memory. The cache is organized in such a way that the least recently used items are removed from the cache so that more frequently accessed items can remain in the cache. It is a form of memory optimization that is used to improve the performance of programs that access large amounts of data.

## What is rate-limiting?

Rate-limiting is a type of control used to limit the rate of requests that a user can make to a server or network in a given period of time. It is used to prevent abuse and maintain quality of service by limiting the demand on system resources and protect against malicious activities such as distributed denial of service (DDoS) attacks. Rate-limiting typically involves limiting user requests to a certain number of requests per second or minute.

## What is a load balancer?

A load balancer is a device that distributes network or application traffic across a cluster of servers. Load balancers improve the performance, availability, and scalability of applications by distributing the workload evenly across multiple servers. This helps ensure that no single server is overwhelmed with requests and that all requests are served promptly and efficiently.

## What is the difference between SQL and NoSQL databases?

SQL databases are relational databases that use Structured Query Language (SQL) to store and retrieve data. They are built for traditional data and are commonly used for transaction processing and data warehousing. NoSQL databases are non-relational databases that use a variety of query languages and data models to store and retrieve data. They are built for large datasets, and are commonly used for applications that require quick access to large amounts of data.

## What is a web socket?

A web socket is a protocol that allows two-way communication between a client and a server over the internet. It is a full-duplex communication channel that operates over a single TCP connection. Web sockets enable real-time exchange of data between client and server and are used to facilitate applications such as online gaming, chat applications, and other collaborative tools.

## Describe how you design an API?

1. Define the scope: First, decide what services and resources the API will provide. This includes defining the types of requests the API will accept and the format of the response.

2. Establish the endpoints: Each endpoint should represent a specific resource or service and should provide a consistent and intuitive way for developers to interact with the API.

3. Choose the data format: Decide on the data format (e.g. JSON, XML, etc.) to be used when making requests and responses.

4. Design the authentication: Decide on the authentication scheme to be used when making requests. This could include an API key, OAuth, or other authentication methods.

5. Build the endpoints: Build out the endpoints with the necessary logic to process requests and return appropriate responses.

6. Test the API: Test the API to make sure it is working as expected and that it meets the needs of the developer.

7. Document the API: Create comprehensive documentation that developers can use to understand and use the API. This includes endpoint descriptions, authentication methods, usage examples, and more.

## What is Redis? Why do we use it?

Redis is an open source, in-memory data structure store used as a database, cache, and message broker. It is often used to improve the performance of web applications by reducing the amount of data that needs to be read from the database, as well as to store transient data such as user sessions and application state. Redis is also used for tasks such as leaderboards and real-time analytics.

## What is a horizontal and vertical scaling?

Horizontal scaling is the process of adding more resources (such as servers or additional storage) to a system in order to increase its capacity. Vertical scaling is the process of increasing the capacity of a single resource (such as increasing the power of a single server's processor or the amount of memory in the server).

## How do you build a system which is reliable?

1. Design a system with redundancy: Redundancy is key to creating reliable systems. By having multiple components that can take over in the event of failure, you can ensure that the system stays running.

2. Leverage fault tolerance: Fault tolerance is a system design strategy that enables a system to continue to operate in the event of a component failure. This can be done through replication, clustering, or other means.

3. Test, test, and test again: System reliability can be improved through thorough testing and validation. Stress testing, load testing, and other tests can help identify and fix potential problems before they cause a system failure.

4. Monitor the system: Regular monitoring of the system can help identify potential issues before they become a problem. This can be done through system logs, performance monitoring, or other means.

5. Implement automated failover: Automated failover is a system design strategy that allows for automatic recovery from system failures. This can help ensure that the system remains available in the event of an outage.



### Node.js

## What is throughput?

Throughput is a measure of the amount of data that can be transmitted or processed within a certain period of time. It is often expressed in terms of bits per second (bps), bytes per second (Bps) or some other unit of information. Throughput is an important factor in the performance of networks, servers and other computing systems.

## what is the difference between readFile and readFileSync

The main difference between readFile and readFileSync is that readFile is asynchronous and readFileSync is synchronous. 

readFile is asynchronous, meaning that it reads a file without blocking the main program from executing other instructions. readFileSync is synchronous, meaning that it blocks the main program until the file is completely read. readFile will return a callback with the content of the file when the read operation is complete, while readFileSync will return the content of the file immediately after it is read.

## How can you make a network request using http module?

You can make a network request using the http module by using the http.get() method, which takes a URL as its argument and returns a stream of the response data. You can also use the http.request() method to make a custom request with options such as the method, headers, and payload. An example of making a GET request using the http.get() method:

const http = require('http');

http.get('http://example.com', (res) => {
    let data = '';
    res.on('data', (chunk) => {
        data += chunk;
    });
    res.on('end', () => {
        console.log(data);
    });
}).on('error', (err) => {
    console.log(err);
});

## What is libuv?

Libuv is a multi-platform support library with a focus on asynchronous I/O. It was primarily developed for use by Node.js, but it's also used by Luvit, Julia, pyuv, and others. Libuv provides a set of core APIs for interacting with the underlying operating system, including asynchronous I/O, threading, timers, and signal handling. It is written in C, and provides bindings for a number of other languages.

## What are the different phases involved in event loop?

The phases involved in the event loop are:

1. Polling: The event loop checks the task queue for any pending tasks that need to be executed.

2. Callback Execution: If a task is found in the queue, the corresponding callback function is executed.

3. Rendering: Once the callback is executed, the event loop will render the changes in the UI.

4. Idle: When there are no tasks in the queue, the event loop will enter an idle state. It will wait for new events to arrive before it can continue.

5. Checking for new tasks: Once the event loop is in its idle state, it will check the task queue for new tasks. If any tasks are found, it will go back to the Polling phase.

## What are timers in Node.js?

Timers in Node.js are functions that execute code after a specified amount of time has elapsed. They are used to delay the execution of a given code block and can be used to create intervals and timeouts. Timers are part of the Node.js Event Loop and are used to schedule code execution.

## What is NVM? how do you use it?

NVM (Node Version Manager) is a command line tool used for installing and managing multiple Node.js versions. It is used to switch between different Node.js versions with ease. To use NVM, you need to install it on your system, then set up the version you would like to use. After that, you can use NVM commands to switch between different versions, install new ones, and more.

## What is common.js? how is it different from es modules?

CommonJS is a module system designed for synchronous loading of modules in a server-side environment. It was designed to provide a method for modularizing code so that code can be shared across multiple applications. CommonJS modules are usually loaded in a synchronous manner, meaning that modules must be loaded in order of dependency.

ES Modules are a newer module system designed for loading modules in an asynchronous manner. They are designed to work in both server-side and client-side environments, and they use static imports and exports to define the module's interface. ES Modules can be loaded asynchronously, meaning that modules can be loaded in any order without affecting the execution of the code.

## How does the crypto module work?

The crypto module in Node.js is a cryptographic library that provides cryptographic functionality for Node.js applications. It includes support for digital signatures, symmetric encryption, message authentication codes, and hash functions. It also provides a set of wrappers for OpenSSL's hash, HMAC, cipher, decipher, sign, and verify functions. The module can be used to create digital signatures, encrypt data, and generate secure random numbers. It can also be used to securely store and retrieve data from databases, and to securely transmit data over networks.

## What are microservices?

Microservices are a type of software architecture that structures an application as a collection of loosely coupled services. This style of architecture is designed to make applications more scalable and easier to maintain. Microservices are developed independently and can be deployed and scaled with relative ease. They are typically built using a range of different programming languages and frameworks.



### Express.js+Mongoose

## How does express work?

Express is a web application framework for Node.js. It provides a set of features that make it easier to write web applications and APIs. It simplifies the process of routing, request handling, input validation, session management, and more. Express is based on the middleware architecture and allows developers to create their own middleware for custom functionality. Express also provides support for templating engines, which makes it easier to render HTML pages with data from the server.

## What are routes?

Routes are a way of describing how a web application responds to a client request to a particular endpoint, which is typically a combination of an HTTP method and a URL path. Routes are used to define the logic of how an application handles various requests, including what data is returned, what view is rendered, or whether a user is authenticated.

## What are Middlewares?

Middlewares are functions that have access to the request and response objects, and are used to modify incoming requests to a web application before they are sent to the route handlers. They are often used for authentication, logging, rate-limiting, and other tasks.

## What is MVC framework?

MVC stands for Model-View-Controller, and it is an architectural software design pattern used in software engineering. The MVC pattern divides an application into three separate layers: the model, the view, and the controller. The model is responsible for managing the data of the application, the view is responsible for displaying that data, and the controller is responsible for responding to user input and controlling the interactions between the model and the view.

## How do you do validations? 

Validations can be done in a variety of ways, depending on the circumstances and the data needed to be validated. Generally, validations are done by checking the data against a set of criteria or rules. This can be done through code, such as with a programming language, or through a third-party service such as an online form validator. Other methods of validating data include using regular expressions, database constraints, or manual review.

## How do you do static routing?

Static routing is the process of manually entering routes into a router’s routing table. To do static routing, the network administrator must configure each router with the necessary static routes. The routes may be manually entered using a command line interface (CLI) or a graphical user interface (GUI). The static routes must include the destination IP address, the subnet mask, the gateway or next hop IP address, and the administrative distance.

## What are some templating engines?

1. Jinja2
2. Mustache
3. EJS
4. Nunjucks
5. Handlebars
6. Dust
7. Haml
8. Pug
9. Swig
10. Smarty

## How do you manage sessions in express?

Express uses a middleware called Express Sessions to manage sessions in the application. This middleware stores session data in a store, which defaults to a memory store. The session data is stored as a cookie on the client side, and the session ID is sent as part of the request. The Express Session middleware can be configured to use other stores such as Redis, MongoDB, or PostgreSQL.

## How do you manage cookies with express?

Express does not directly manage cookies, as it is a web application framework. However, you can use a library such as cookie-parser to help you manage cookies in an Express application. Cookie-parser allows you to parse, sign, and serialize cookies from the request and response objects in Express.

## What are common libraries you work with express?

Some of the most popular libraries used with Express are:
-Express-Validator: for data validation 
-Express-Handlebars: for templating 
-Morgan: for logging 
-Cookie-Parser: for cookie management 
-Body-Parser: for parsing request bodies 
-Multer: for file uploads
-CSurf: for CSRF protection 
-Passport: for authentication 
-Helmet: for security-related HTTP headers.

## What is CORS?

CORS (Cross Origin Resource Sharing) is a mechanism that enables web browsers to send and receive data from resources located on a different domain than the one the page is hosted on. CORS allows websites to access resources from other domains without needing to bypass the same origin policy.

## What are Models in mongoose?

Models in mongoose are JavaScript objects that represent a collection of documents in a MongoDB database. They are used to define the structure, data types, and validation for a collection and can also be used to create, read, update, and delete documents.

## Explain why mongoose does not return a promise but has a .then()

Mongoose does not return a promise because it does not have an inbuilt promise library. Instead, it uses the Node.js callback pattern. This means that when you call a mongoose method, you pass in a callback function that will be called when the operation has completed. The .then() method is used to convert the mongoose callback into a promise, so that it can be used with Promise based code.

##  What are aggregation pipelines with mongoose?

Aggregation pipelines are a feature of Mongoose, an object data modeling library for MongoDB, which allow developers to define data transformations over a collection. Aggregation pipelines allow developers to perform operations such as sorting, filtering, grouping, and transforming data in order to produce an aggregated result. Aggregation pipelines are a powerful tool that can be used to analyze large datasets, and are an essential part of building modern data-driven applications.

## I'm using an arrow function for a virtual, middleware, getter/setter, or method and the value of this is wrong. Why?

Most likely, your arrow function is not correctly configured. Arrow functions are often used to create a "this" context in which a function or method is executed, and if the arrow function is not correctly configured, the "this" context may be incorrect. Additionally, arrow functions may not be able to correctly capture arguments and other data, which can lead to incorrect values. Make sure that the arrow function is configured correctly before using it.

## Should I create/destroy a new connection for each database operation?

No, it is not recommended to create and destroy a new connection for each database operation. Creating and destroying a new connection for each database operation can be inefficient, costly, and time consuming. Instead, it is recommended to use connection pooling to maintain a pool of database connections that can be reused. This will allow the database operations to be performed more quickly and efficiently.

## My query/update seems to execute twice. Why is this happening?

There could be several different causes for this issue. It could be a result of a database trigger, a coding error, or an issue with the database server itself. It is best to consult your database administrator or a database expert to determine the exact cause.

## How do you create indexes with mongoose? 

Indexes can be created with mongoose using the Schema.index() method. This method takes two arguments, the first being an array of fields to be indexed and the second being an object containing the index options. For example:

const schema = new mongoose.Schema({
  name: { type: String },
  age: { type: Number },
});

schema.index({ name: 1, age: -1 }, { unique: true });

## What are pre and post hooks?

Pre and post hooks are functions that execute before and after a certain event, respectively. Pre hooks are used to perform some kind of task before the event occurs, while post hooks are used to perform some kind of task after the event has taken place. Pre and post hooks are often used to ensure that certain tasks are completed before and after an event, such as validating user input before executing a process or sending out notifications after a process has been completed.