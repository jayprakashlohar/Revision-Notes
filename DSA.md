## What is Bubble sort ?

Bubble sort is a simple sorting algorithm that repeatedly compares adjacent elements in a list and swaps them if they are in the wrong order. It continues this process until the entire list is sorted. The largest (or smallest) elements "bubble" to the end (or beginning) of the list with each iteration, hence the name "bubble sort."

## What is Selection sort?

Selection sort is a simple sorting algorithm that divides the input list into two portions: the sorted portion and the unsorted portion. It repeatedly selects the smallest (or largest) element from the unsorted portion and swaps it with the first element of the unsorted portion. This process continues until the entire list is sorted.

## What is the meaning of the Stack Data Structure ?

A stack is a data structure that follows the principle of Last-In-First-Out (LIFO). It works like a stack of objects, where the last object added is the first one to be removed. Elements can only be added or removed from the top of the stack. This is commonly referred to as push (addition) and pop (removal) operations. Think of a stack of plates, where you can only add or remove plates from the top. Stacks are often used in programming for tasks like managing function calls, keeping track of program execution, and handling undo/redo operations.

## What is the meaning of the Queue Data Strucxture?

A queue is a data structure that follows the principle of First-In-First-Out (FIFO). It functions like a queue of people waiting in line, where the first person who joins the queue is the first one to be served. Elements can only be added at the rear end of the queue (enqueue) and removed from the front end (dequeue). This ensures that elements are processed in the same order they were added. Queues are commonly used in scenarios such as managing tasks, scheduling processes, and implementing breadth-first search algorithms.

## Write a program to move all 0's to the end of the array?

function moveZerosToEnd(arr) {
for (let i = 0; i < arr.length; i++) {
if (arr[i] === 0) {
arr.splice(i, 1); // Remove the zero element at index i
arr.push(0); // Add a zero element at the end
i--; // Decrement the index to recheck the current position
}
}

return arr;
}

// Example usage
const array = [0, 1, 0, 3, 12];
console.log(moveZerosToEnd(array)); // Output: [1, 3, 12, 0, 0]

## what does Intellipaat do?

Intellipaat is an online learning platform that offers a wide range of courses and training programs in various technologies, including data science, artificial intelligence, cloud computing, programming languages, and more. It provides industry-relevant, self-paced, and instructor-led training to help individuals enhance their skills and gain expertise in their chosen fields. Intellipaat aims to make quality education accessible to everyone and empowers learners with the knowledge and skills needed to excel in their careers.

## Why do you want to join Intellipaat ?

I am excited to join Intellipaat because I believe it is the best online learning platform for professionals who want to upskill and stay ahead of the curve in the technical support field. Intellipaat offers a wide range of courses in the most in-demand technologies, taught by industry experts. The courses are highly interactive and engaging, and Intellipaat also offers lifetime access to course material and support.

I am also drawn to Intellipaat's culture of innovation and its commitment to helping learners succeed. I believe that Intellipaat is a great place to work and grow my career. I am confident that I can make a significant contribution to Intellipaat's team and help the company achieve its goals.