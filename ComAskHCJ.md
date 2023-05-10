### GENERAL QUESTIONS

## What is your strength as a developer?

My strength as a developer is my ability to quickly understand new technologies, adapt to new environments, and work well with team members. I have a knack for problem solving, and I enjoy learning new programming languages. I am also highly organized and detail-oriented, and I take great pride in my work.

## What are your salary expectations?

My salary expectations are dependent on the job requirements and what I can bring to the role. I am confident in my abilities and willing to discuss the specifics with you during the interview process.

## How much relocation time is required?

The amount of relocation time required depends on a number of factors such as the distance of the move, the size of the home and the amount of belongings being moved. Generally, it can take anywhere from two days to two weeks to complete a relocation.

## If the company did lay-off you after five years, what would you do in this situation?

If I were laid off after five years with a company, I would first assess the reasons for the lay-off. If it was due to restructuring or downsizing, I would look for other opportunities in the same or a similar field. I would also take the time to update my resume, network with contacts, and look into any training or educational opportunities that could help me find a new job. Additionally, I would look into any unemployment benefits that may be available to me.

## Where do you see yourself in 5 years?

In 5 years, I hope to have achieved my professional goals and be in a position of leadership where I can use my expertise to help others. I also hope to have explored more of the world and be in a place of financial security.

### HTML AND CSS

## HTML CSS task: Create a box and center it in the viewport?

HTML:

<div class="box">
  Content here
</div>

CSS:
.box {
width: 300px;
margin-left: auto;
margin-right: auto;
padding: 10px;
border: 1px solid #000;
text-align: center;
}

## What is a css preprocessor?

A CSS preprocessor is a program that takes a basic CSS file and compiles it into a more efficient, browser-friendly version. This allows developers to write more complex stylesheets and make changes more quickly. It also adds features such as variables, mixins, and nesting structures to the stylesheets, making them easier to read and maintain.

## Clone some static part of the given web page

<div class="static-part">
  <div class="logo">
    <img src="images/logo.png" alt="Company Logo" />
  </div>
  <div class="navigation">
    <ul>
      <li><a href="index.html">Home</a></li>
      <li><a href="about.html">About Us</a></li>
      <li><a href="services.html">Services</a></li>
      <li><a href="contact.html">Contact Us</a></li>
    </ul>
  </div>
</div>

## Types of @media rules in CSS?

1. @media screen: Used for computer screens, tablets, smart-phones etc.
2. @media print: Used for printed documents.
3. @media speech: Used for screen readers that “read” the page out loud.
4. @media all: Used for all media types.
5. @media aural: Used for speech and sound synthesizers.
6. @media braille: Used for braille tactile feedback devices.
7. @media embossed: Used for paged braille printers.
8. @media handheld: Used for handheld devices like smartphones.
9. @media projection: Used for projected presentations, like slides.
10. @media tty: Used for media using a fixed-pitch character grid, like teletypes and terminals.
11. @media tv: Used for television-type devices.

### JAVASCRIPT

## What are the methods of debugging and testing?

Debugging:

1. Print Statements: Inserting print statthe ements in code to track execution of program.
2. Step Through Debugging: Step-by-step debugging of code to help identify the source of errors.
3. Breakpoints: Setting breakpoints in code to pause the execution at specific lines of code.
4. Debugger: Using a debugger tool to identify and fix errors.
5. Logging: Inserting logging statements in code to track the execution of the program.

Testing:

1. Unit Testing: Testing individual components of a system to ensure they are working as expected.
2. Integration Testing: Testing how components interact with each other in a system.
3. Functional Testing: Testing the functional requirements of a system.
4. Performance Testing: Testing the performance of a system under different conditions.
5. Stress Testing: Testing the system's ability to handle extreme loads.
6. Usability Testing: Testing the user experience of a system.
7. Regression Testing: Testing to ensure that changes have not introduced bugs into the system.

## What is the Var, let and const?

Var is used to declare a variable and is function-scoped. This means that the variable is accessible throughout the function and can be modified, reassigned, and deleted.

Let is used to declare a variable and is block-scoped. This means that the variable is only accessible within the block of code in which it was declared and can be modified, reassigned, and deleted.

Const is used to declare a variable and is block-scoped. This means that the variable is only accessible within the block of code in which it was declared and cannot be modified, reassigned, or deleted.

## What are the Ways to create objects?

1. Constructor: The most common way to create an object is by using the new keyword with a constructor method. This method uses the class keyword to define the object type and then creates a new instance of the object.

2. Object.create(): This is a static method that creates a new object, using an existing object as the prototype of the newly created object.

3. Literal Notation: This is a shorthand way of creating an object without using a constructor or object.create(). It uses curly braces to define an object and its properties.

4. Function Constructors: A function can be used as a constructor to create an object. It is similar to the constructor approach, but instead of using the class keyword, you use the function keyword.

5. Factory Functions: A factory function is a function that returns a new object. The advantage of using a factory function is that you can easily create multiple similar objects without having to manually define each one.

## Create a object using constructor?

function Person(name, age, job) {
this.name = name;
this.age = age;
this.job = job;
}

const person1 = new Person('John', 25, 'Developer');

## What is Hoisting in javascript?

Hoisting is a JavaScript mechanism where variables and functions are moved to the top of their scope before code execution. This means that no matter where functions and variables are declared, they are moved to the top of their scope regardless of whether their scope is global or local. Hoisting helps to give JavaScript its functional scope.

## Difference between Normal function and arrow function ?

A normal function is declared using the function keyword, and can have its own this, arguments, super, and new.target. An arrow function is declared using the fat arrow (=>) and does not have its own this, arguments, super, or new.target. Arrow functions are also more concise and easier to read than normal functions.

## write the number in words?

One hundred seventy-five

## Print prime numbers up to n numbers.?

//Solution

function printPrimeNumbers(n) {
for (let i = 2; i <= n; i++) {
let isPrime = true;
for (let j = 2; j < i; j++) {
if (i % j === 0) {
isPrime = false;
break;
}
}
if (isPrime) console.log(i);
}
}

printPrimeNumbers(20);

## What is a higher order function?

A higher order function is a function that takes one or more functions as arguments and/or returns a function as its result. It is a function that operates on other functions, either by taking them as arguments or by returning them.

## What is Ref?

Ref is short for reference. It is an object or variable that stores a reference to another object or variable. It is commonly used in programming languages such as JavaScript, Python, and Java.

## Create a function to return the longest word in a string?

in javascript

function longestWord(str) {
let words = str.split(' ');
let longest = '';

for (let word of words) {
if (word.length > longest.length) {
longest = word;
}
}

return longest;
}

## Input:dummy text of the printing and typesetting industry ?

Answer: Lorem Ipsum is the standard dummy text of the printing and typesetting industry. It has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.

## Output: typesetting

Definition: Typesetting is the arrangement of text and images on a page or document. It involves the selection of typefaces, point sizes, line lengths, line-spacing, and letter-spacing, as well as the adjustment of space between pairs of letters, words, and lines of text. Typesetting is a key component of the publishing process.

## Write a program that accepts an email string and validates that email. If email is valid must

display success message and If email is not valid must display error message?

in javascript

function validateEmail(email) {
const re = /^(([^<>()\[\]\\.,;:\s@"]+(\.[^<>()\[\]\\.,;:\s@"]+)\*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/;
if (re.test(email)) {
return true;
}
return false;
}

let email = "example@email.com";

if (validateEmail(email)) {
console.log("Email is valid!");
} else {
console.log("Email is not valid!");
}

## What is recursion?

Recursion is a process in which a function calls itself directly or indirectly. This allows the function to repeat itself until a certain condition is met. Recursion is useful for tasks that can be defined in terms of similar sub-tasks.

## What is time complexity?

Time complexity is a measure of the amount of time it takes for a computer algorithm to run. It is usually expressed using Big O notation which takes into account the time it takes for the algorithm to run as the input size increases.

## Find the smallest negative element in array?

code in js

let arr = [1, -4, -7, 8, -12];

let smallestNegative = arr.reduce((acc, curr) => {
return Math.min(acc, curr);
}, 0);

console.log(smallestNegative); // output: -12

## Difference between java and javascript?

Java is a programming language that is compiled and run on a virtual machine. It is mainly used for server-side development, creating applications and websites. JavaScript is a scripting language that runs inside a web browser. It is mainly used for client-side development, creating interactive web pages and web applications.

##
