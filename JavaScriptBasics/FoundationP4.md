Using arrays.
Using built-in array methods.
Using loops.
Getting your hands dirty with TDD exercises.



####1. Using arrays:
Overview:
Arrays are used to store multiple values in a single variable.
They are ordered, indexed, and can hold various data types.
Arrays provide methods for manipulation and iteration.
Declaration:
```
// Example:
var fruits = ["Apple", "Banana", "Orange"];
```

#### 2. Using built-in array methods:
Overview:
JavaScript provides built-in methods for working with arrays.
Common methods include push, pop, shift, unshift, splice, slice, forEach, map, filter, etc.
Example:
```
// Adding elements to the end of an array
fruits.push("Mango");

// Removing the last element
var removedFruit = fruits.pop();

// Iterating over elements
fruits.forEach(function(fruit) {
  console.log(fruit);
});
```

### 3. Using loops:
Overview:
Loops are used to repeatedly execute a block of code.
Common loop types are for, while, and do-while.
Loops help iterate over arrays or perform tasks a specific number of times.
```
// For loop
for (var i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}

// While loop
var i = 0;
while (i < fruits.length) {
  console.log(fruits[i]);
  i++;
}
```

### 4. Getting your hands dirty with TDD exercises:

Overview:
Test-Driven Development (TDD) is a software development approach where tests are written before the code.
It involves three steps: writing a failing test, writing the minimum code to pass the test, and then refactoring.

Examples:
Assume we are building a simple function to add two numbers.
Step 1: Write a Failing Test
```
// Test Case
test("Adding 2 + 3 should return 5", function() {
  assert.equal(add(2, 3), 5);
});
```
Step 2: Write Minimum Code to Pass the Test
```
// Function Implementation
function add(a, b) {
  return a + b;
}
```
Step 3: Refactor (if needed)
Refactor the code to improve readability or performance while ensuring the test still passes.
This cycle continues as you add more features or make changes, ensuring that your code remains reliable.


____

### 1 . What is an array?

Definition:
An array is a data structure in JavaScript that allows you to store and organize multiple values under a single variable.
```
var fruits = ["Apple", "Banana", "Orange"];
```

### 2. What are arrays useful for?
Overview:
Arrays are useful for storing and managing collections of data.
They provide an ordered and indexed structure for elements.

### 3. How do you access an array element?
Accessing Elements:
Use square brackets [] with the index to access array elements. Indexing starts from 0.
Example:
```
var firstFruit = fruits[0]; // Accessing the first element ("Apple")


```

### 4. How do you change an array element?
Modifying Elements:
Use the index to access the element and assign a new value.
Example:
```
fruits[1] = "Grapes"; // Changing the second element to "Grapes"

```
### 5. What are some useful array properties?
Useful Properties:
length: Returns the number of elements in the array.
Example:
```
var arrayLength = fruits.length; // Returns the length of the array (3)

```

### 6. What are some useful array methods?
Useful Methods:
push, pop, shift, unshift, splice, slice, forEach, map, filter, etc.
Example:
```
fruits.push("Mango"); // Adds "Mango" to the end of the array
```

### 7. What are loops useful for?
Overview:
Loops are useful for executing a block of code repeatedly.
They are handy for iterating over array elements or performing repetitive tasks.

### 8. What is the break statement?
Break Statement:
The break statement is used to exit a loop prematurely.
Example:
```
for (var i = 0; i < 10; i++) {
  if (i === 5) {
    break; // Exits the loop when i is 5
  }
  console.log(i);
}

```
### 9. What is the continue statement?
Continue Statement:
The continue statement skips the current iteration of a loop and moves to the next one
```
for (var i = 0; i < 5; i++) {
  if (i === 2) {
    continue; // Skips the iteration when i is 2
  }
  console.log(i);
}

```

### 10. What is the advantage of writing automated tests?

###### Advantages of Automated Tests:
Detect and prevent software bugs early in the development process.
Ensure code changes don't introduce new issues (regression testing).
Improve code quality and maintainability.
Facilitate collaboration among team members.
Provide documentation for expected behavior.
Boost confidence in making changes and refactoring code.

