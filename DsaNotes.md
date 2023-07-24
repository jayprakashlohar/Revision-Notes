### data structures and algorithms

## What is data structures and algorithms ?

Data structures and algorithms are a fundamental part of computer science. Data structures are a way of organizing and storing data so that it can be accessed and modified in an efficient manner. Algorithms are a set of instructions that take an input, process it and produce an output. They are used to solve problems and are the basis of computer programming.

## what is bubble sort?

Bubble sort is a sorting algorithm that repeatedly steps through a list, compares adjacent elements and swaps them if they are in the wrong order. It is one of the simplest sorting algorithms and is often used to sort small lists of numbers. Bubble sort has a worst-case and average complexity of O(n2), where n is the number of items being sorted.

## what is selection sort?

Selection sort is an in-place sorting algorithm that works by repeatedly finding the minimum element from the unsorted portion of the list and moving it to the beginning of the list. This process is repeated until the list is sorted.
Selection Sort has a time complexity of O(n^2) and a space complexity of O(1).

## what is merge sort?

Merge sort is a divide and conquer sorting algorithm that works by recursively breaking down a larger list of items into smaller, more manageable lists and then combining them in a way that creates a sorted list. The time complexity of Merge Sort is O(n log n) in all 3 cases (worst, average and best) as merge sort always divides the array into two halves and takes linear time to merge two halves. The space complexity of Merge Sort is O(n) which makes it relatively space efficient.

## what is quick sort ?

Quick Sort is a sorting algorithm that sorts an array of elements by dividing it into two subarrays, the first subarray containing elements that are less than or equal to a pivot element, and the second subarray containing elements that are greater than the pivot element. The algorithm then recursively sorts each subarray until the entire array is sorted. Quick Sort is typically faster than Bubble Sort and Insertion Sort, and is often used in practice.

Time Complexity: O(nlog(n))
Space Complexity: O(log(n))

## what is queue?

Queue is a linear data structure where the first element is inserted from one end called REAR and deleted from the other end called FRONT. It follows a First-In-First-Out (FIFO) structure, meaning that the item that is inserted first is the first one to be removed.

## what is stack?

A stack is a linear data structure that follows the Last In First Out (LIFO) principle. It is a collection of objects that are inserted and removed from the same end, with the most recently added item being the first one to be removed. The stack is a basic data structure that is used to store data for quick access, sorting, reversing, and other operations.

## what is the time and space compacity of stake?

The time and space complexity of a stack depends on the operations that are performed. Generally, the time complexity of a stack is O(1) for basic operations such as push, pop, peek, and isEmpty. The space complexity of a stack is O(n), where n is the number of items in the stack.

## what is the space and time complexity of the queue?

The space complexity of a queue is O(n), where n is the number of elements in the queue. The time complexity of the most common operations on a queue (enqueue and dequeue) is O(1).

## what are the time and space complexity of recursion?

Time complexity of recursion is usually exponential, or O(2^n). Space complexity of recursion is O(n) in the worst case, where n is the depth of recursion.

<!-- ---------------------- ------------------------ ------------------------- ----------------------- --------- -->

## Remove Duplicates from Sorted Array ?

<!-- let arr = [1,1,2,2,3,3,4,4,5,5,5,5,5]
  function print(arr) {
    let unique = [];
    for (let i = 0; i < arr.length; i++) {
      if (arr[i] !== arr[i + 1]) {
        unique.push(arr[i]);
      }
    }
    console.log(unique)
  }
print(arr); -->

## Rotate Array?

<!-- // Rotate array clockwise
function rotateArray(arr) {
  let last = arr.pop();
  arr.unshift(last);
  return arr;
}

// Rotate array counter-clockwise
function rotateArray(arr) {
  let first = arr.shift();
  arr.push(first);
  return arr; -->

}

## Given an array, does an array Contains Duplicate ?

<!-- function hasDuplicates(arr) {
  for(let i = 0; i < arr.length; i++) {
    for(let j = i + 1; j < arr.length; j++) {
      if(arr[i] === arr[j]) {
        return true;
      }
    }
  }
  return false;
} -->

## Given a non-empty array of integers nums, every element appears twice except for one. Find that single one?

<!--
function print(arr) {
 let res = 0
for(let i = 0; i < arr.length; i++) {
    res^= arr[i]
  }
  console.log(res)
}
print(arr) -->

## The intersection of two arrays?

<!-- const array1 = [1, 2, 3, 4, 5];
const array2 = [3, 4, 5, 6, 7];
const intersection = array1.filter(value => array2.includes(value));
console.log(intersection); // Output: [3, 4, 5] -->

## Difference of two arrays?

<!-- //Using the spread operator
const array1 = [1, 2, 3, 4];
const array2 = [3, 4, 5, 6];
const difference = [...array1].filter(x => !array2.includes(x));
console.log(difference); // [1, 2] -->

---

<!-- for (let i=0; i<arrayA.length; i++) {
    let element = arrayA[i];

    if (!arrayB.includes(element)) {
        console.log(element);
    }
} -->

## Given an array of numbers [1,2,3...] you need to add another number n to it

for example [1,2,3] + 12 = [1,3,5]

<!-- var numbers = [1, 2, 3];
var n = 2;
function print(numbers) {
  for (var i = 0; i < numbers.length; i++) {
    numbers[i] += n;
  }
  console.log(numbers);
}
print(numbers) -->

## Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target?

<!-- function twoSum(nums, target) {
  let result = [];
  for(let i=0;i<nums.length;i++){
      for(let j=i+1; j<nums.length;j++) {
          if(nums[i] + nums[j] === target) {
              result.push(i,j);
          }
      }
  }
  return result;
} -->

## You are given an n x n 2D matrix representing an image, rotate the image by 90 degrees?
<!-- function rotateMatrix(matrix) { 
  const N = matrix.length; 
  const rotatedMatrix = []; 
  // loop through the matrix 
  for (let i = 0; i < N; i++) { 
    rotatedMatrix.push([]); 
    for (let j = 0; j < N; j++) { 
      rotatedMatrix[i].push(matrix[N - j - 1][i]); 
    } 
  } 
  return rotatedMatrix; 
} -->

## Flatten an array ?
<!-- function flattenArray(arr) {
  return arr.reduce(function(prev, curr) {
    return prev.concat(Array.isArray(curr) ? flattenArray(curr) : curr);
  }, []);
} -->

## Given an array of strings strs, group the anagrams together. You can return the answer in any order?

<!-- const groupAnagrams = (strs) => {
  let anagrams = {};
  for (let str of strs) {
    let sortedStr = str.split('').sort().join('');
    if (anagrams[sortedStr] === undefined) {
      anagrams[sortedStr] = [str];
    } else {
      anagrams[sortedStr].push(str);
    }
  }
  return Object.values(anagrams);
} -->

## Longest Substring Without Repeating Characters?

<!-- function findLongestSubstring(str) {
  let longest = 0;
  let seen = {};
  let start = 0;
 
  for (let i = 0; i < str.length; i++) {
    let char = str[i];
    if (seen[char]) {
      start = Math.max(start, seen[char]);
    }
    // index - beginning of substring + 1 (to include current in count)
    longest = Math.max(longest, i - start + 1);
    // store the index of the next char so as to not double count
    seen[char] = i + 1;
  }
  return longest;
} -->

## Longest Palindromic Substring?
<!-- 
function longestPalindrome(string) {
  let longest = '';
  for (let i = 0; i < string.length; i++) {
    for (let j = 0; j < 2; j++) {
      let left = i;
      let right = i + j;
      while (string[left] && string[left] === string[right]) {
        left--;
        right++;
      }
      if ((right - left - 1) > longest.length) {
        longest = string.substring(left + 1, right);
      }
    }
  }
  return longest;
} -->

## Longest increasing subsequence?

<!-- // This function finds the length of the longest increasing subsequence
// in an array of numbers
function findLongestIncreasingSubsequence(arr) {
  let maxLength = 0;
  let tempLength = 0;

  // Loop through each element in the array
  for (let i = 0; i < arr.length; i++) {
    tempLength = 1;

    // Compare the current element with the elements to its left
    for (let j = i - 1; j >= 0; j--) {
      // If the element to its left is smaller, then increment the tempLength
      if (arr[j] < arr[i]) {
        tempLength++;
      }
    }

    // Keep track of the maxLength
    if (tempLength > maxLength) {
      maxLength = tempLength;
    }
  }

  return maxLength;
} -->

## how to find Maximum sum of SubArray ?
<!-- function maxSumSubArray(arr) {
  let maxSum = 0;
  let currentSum = 0;

  for (let i = 0; i < arr.length; i++) {
    currentSum += arr[i];
    if (currentSum > maxSum) {
      maxSum = currentSum;
    }
    
    if (currentSum < 0) {
      currentSum = 0;
    }
  }
  return maxSum;
} -->

## Find Consonants in a String ?
<!-- 
let str = "masai"
function getConsonants(str) {
  // declare consonants string
  let consonants = '';
  // loop through each character in the string
  for (let i = 0; i < str.length; i++) {
    // get the character
    let char = str[i];
    // check if the character is a consonant
    if (
      char !== 'a' &&
      char !== 'e' &&
      char !== 'i' &&
      char !== 'o' &&
      char !== 'u'
    ) {
      // if it is, add it to the consonants string
      consonants += char;
    }
  }
  // return the consonants
 
  console.log(consonants)
}

getConsonants(str) -->

##  Compare Two Array - find missing ?

<!-- function compareArrays(arr1, arr2) {
  let missing = [];
  for (let i = 0; i < arr1.length; i++) {
    if (!arr2.includes(arr1[i])) {
      missing.push(arr1[i]);
    }
  }
  return missing;
} -->

##  Find All the Maximum and Minimum element in Array?
<!-- // To find the maximum element in an array:

// using Math.max()
const array = [1, 2, 3, 4, 5];
const maxElement = Math.max(...array);
console.log(maxElement); // Output: 5

// using reduce()
const array = [1, 2, 3, 4, 5];
const maxElement = array.reduce((a, b) => Math.max(a, b));
console.log(maxElement); // Output: 5

// To find the minimum element in an array:

// using Math.min()
const array = [1, 2, 3, 4, 5];
const minElement = Math.min(...array);
console.log(minElement); // Output: 1

// using reduce()
const array = [1, 2, 3, 4, 5];
const minElement = array.reduce((a, b) => Math.min(a, b));
console.log(minElement); // Output: 1 -->

## Find second largest and smallest element in array?
<!-- // To find the second largest element in the array: 

let myArray = [2,5,7,10,12,15];

// Sort the array in descending order
let sortedArray = myArray.sort(function(a, b){return b - a});

// Get the second largest element from the sorted array
let secondLargest = sortedArray[1];

console.log(secondLargest); // Output: 12


// To find the second smallest element in the array:

let myArray = [2,5,7,10,12,15];

// Sort the array in ascending order
let sortedArray = myArray.sort(function(a, b){return a - b});

// Get the second smallest element from the sorted array
let secondSmallest = sortedArray[1];

console.log(secondSmallest); // Output: 5 -->

<!-- ## 
function minJump(arr) { 
   let jumps = new Array(arr.length); 
  
   if (arr.length == 0 || arr[0] == 0) 
     return -1; 
  
   jumps[0] = 0; 
  
   for (let i = 1; i < arr.length; i++) 
   { 
     jumps[i] = Number.MAX_VALUE; 
     for (let j = 0; j < i; j++) 
     { 
       if (i <= j + arr[j] && jumps[j] != Number.MAX_VALUE) 
       { 
          jumps[i] = Math.min(jumps[i], jumps[j] + 1); 
          break; 
       } 
     } 
   } 
  
   return jumps[arr.length-1]; 
} 

console.log(minJump([1, 3, 5, 8, 9, 2, 6, 7, 6, 8, 9])); -->


