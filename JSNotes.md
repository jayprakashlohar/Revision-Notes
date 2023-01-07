##HTML,CSS And JavaScript Basic

#What is data structure explain?
_A data structure is a specialized format for organizing, processing, retrieving and storing data. There are several basic and advanced types of data structures, all designed to arrange data to suit a specific purpose. Data structures make it easy for users to access and work with the data they need in appropriate ways._

#What is an Array?
_An array is a collection of items of same data type stored at contiguous memory locations.
This makes it easier to calculate the position of each element by simply adding an offset to a base value, i.e., the memory location of the first element of the array (generally denoted by the name of the array). The base value is index 0 and the difference between the two indexes is the offset._

#what is self closing tag in html?
_Some HTML tags (like img and br ) don't have their own content. These are known as self closing tags or empty tags. They look like this: A simple example: <br /> The br tag inserts a line break (not a paragraph break)._

#what is default value of position property?
_CSS Position: Static Value
This is the default value for the CSS position property. In this mode, the target element is positioned along with the natural document flow. Note that the top, right, bottom, left, as well as z-index properties will not display any effects_

#What is a setAttribute in JavaScript?
_The setAttribute() method sets a new value to an attribute. If the attribute does not exist, it is created first._
_element.setAttribute("class", "democlass");_

#What is a settimeout in js?
_The global setTimeout() method sets a timer which executes a function or specified piece of code once the timer expires._
EXAMLE -
_setTimeout(() => {
console.log("Delayed for 1 second.");
}, 1000)_

#what is setinterval in javascript?
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

#Window clearInterval()?
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

#HTTP Methods?
_GET
POST
PUT
HEAD
DELETE
PATCH
OPTIONS
CONNECT
TRACE_

#What is HTTP?
_The Hypertext Transfer Protocol (HTTP) is designed to enable communications between clients and servers.
HTTP works as a request-response protocol between a client and server.
Example: A client (browser) sends an HTTP request to the server; then the server returns a response to the client._

#Diffrent between HTTP AND HTTPS IN JS ?

- 1. HyperText Transfer Protocol (HTTP): HyperText Transfer Protocol (HTTP) is a protocol using which hypertext is transferred over the Web. Due to its simplicity, http has been the most widely used protocol for data transfer over the Web but the data (i.e. hypertext) exchanged using http isn’t as secure as we would like it to be. In fact, hyper-text exchanged using http goes as plain text i.e. anyone between the browser and server can read it relatively easily if one intercepts this exchange of data.

2. Hypertext Transfer Protocol Secure (HTTPS): Hypertext Transfer Protocol Secure (HTTPS) is an extension of the Hypertext Transfer Protocol (HTTP). It is used for secure communication. In HTTPS, the communication protocol is encrypted using Transport Layer Security. \*

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
10. HTTP does not use data hashtags to secure data. While HTTPS will have the data before sending it and return it to its original state on the receiver side.\*

#What is promiss ?
\*A Promise is a proxy for a value not necessarily known when the promise is created. It allows you to associate handlers with an asynchronous action's eventual success value or failure reason. This lets asynchronous methods return values like synchronous methods: instead of immediately returning the final value, the asynchronous method returns a promise to supply the value at some point in the future.

A Promise is in one of these states:

pending: initial state, neither fulfilled nor rejected.
fulfilled: meaning that the operation was completed successfully.
rejected: meaning that the operation failed.\*
