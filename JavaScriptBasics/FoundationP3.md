1. How to define and invoke different kinds of functions:
Function Definition:

Functions are defined using the function keyword, followed by a name, parameters (if any), and a code block.
Example:
```
function greet(name) {
  console.log("Hello, " + name + "!");
}
```

### Function Invocation:
Functions are invoked (called) by using their name followed by parentheses, and providing any required arguments.
Example:
```
greet("Charly"); // Invoking the greet function
```


### Different Kinds of Functions:
Functions can be named or anonymous.
They can also be assigned to variables (function expressions) or stored in objects (methods).

## 2. How to use the return value:
Return Value:
The return statement is used to send a value back from a function.
Functions can return a single value or an object, array, etc.
Example:
```
function add(a, b) {
  return a + b;
}

var result = add(3, 5); // The returned value (8) is stored in the 'result' variable.
```


###3. What function scope is:
Function Scope:
Function scope refers to the visibility and accessibility of variables within a function.
Variables declared inside a function are local to that function and cannot be accessed outside of it.
Example:
```
function exampleFunction() {
  var localVar = "I am local";
  console.log(localVar);
}

exampleFunction(); // Outputs "I am local"
console.log(localVar); // Error: localVar is not defined (outside the function)
```

### Block Scope (ES6 and later):
The introduction of let and const in ES6 allows for block-scoped variables, providing more fine-grained control over variable visibility.


___

1. What are functions useful for?
Functions are useful for organizing and reusing code. They allow you to define a set of instructions under a name, making it easy to call and execute that set of instructions whenever needed.

2. How do you invoke a function?
To invoke (call) a function, use its name followed by parentheses, and provide any required arguments.
Example:
```
function greet(name) {
    console.log("Hello, " + name + "!" );
}

greet("Charly"); //Invoke the greet function


```


### 3. What are anonymous functions?
Anonymous functions are functions without a specified name. They are often used as inline or callback functions.
```
// Example:
var add = function(a, b) {
  return a + b;
};


```

### 4. What is function scope?
Function scope refers to the visibility and accessibility of variables within a function. Variables declared inside a function are local to that function.
```
// Example:
function exampleFunction() {
  var localVar = "I am local";
  console.log(localVar);
}

```

### 5. What are return values?
Return values are values that a function sends back after execution using the return keyword. They allow a function to provide a result or output.
```
// Example:
function add(a, b) {
  return a + b;
}

var result = add(3, 5); // 'result' holds the returned value (8)
```

### 6. What are arrow functions?
Arrow functions are a concise way to write functions in JavaScript introduced in ES6. They have a shorter syntax compared to traditional function expressions.
```
// Example:
var add = (a, b) => a + b;
```
Arrow functions are often used for short, one-line operations and have an implicit return.
