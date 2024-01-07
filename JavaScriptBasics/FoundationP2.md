Name the eight data types in JavaScript.
Understand the difference between single, double, and backtick quotes.
Embed a variable/expression in a string.
Understand what a method is.
Name the three logical operators.
Understand what the comparison operators are.
Understand what conditionals are.
Understand what nesting is.
Understand what truthy and falsy values are.

1. 
Name the eight data types in JavaScript:
```
var numberExample = 42;             // Number
var stringExample = "Hello";        // String
var booleanExample = true;          // Boolean
var undefinedExample = undefined;   // Undefined
var nullExample = null;             // Null
var objectExample = { key: "value" };// Object
var arrayExample = [1, 2, 3];        // Array
var symbolExample = Symbol("desc");  // Symbol

```

2.
Understand the difference between single, double, and backtick quotes:
```
var singleQuotes = 'Single quotes';
var doubleQuotes = "Double quotes";
var backtickQuotes = `Backtick quotes allow ${1 + 1} expressions`;

```
3.
 Embed a variable/expression in a string:
 ```
 var name = "John";
var age = 25;
var message = `My name is ${name}, and I am ${age} years old.`;

 ```

4.
Understand what a method is:
```
var person = {
  name: "Alice",
  greet: function() {
    console.log(`Hello, ${this.name}!`);
  }
};

person.greet(); // Calls the greet method

```

5.
Name the three logical operators:
```
var x = true;
var y = false;

var logicalAnd = x && y; // false
var logicalOr = x || y;  // true
var logicalNot = !x;     // false
```

6.
 Understand what the comparison operators are:
 ```
 var a = 5;
var b = "5";

var equal = a == b;        // true (performs type coercion)
var strictEqual = a === b;  // false (strict equality, no type coercion)
var notEqual = a != b;      // false (performs type coercion)
var strictNotEqual = a !== b;// true (strict inequality, no type coercion)
var greaterThan = a > 3;    // true
var lessThan = a < 10;      // true
var greaterOrEqual = a >= 5;// true
var lessOrEqual = a <= 5;   // true

 ```

7.
Understand what conditionals are:
```
var condition = true;

if (condition) {
  console.log("This code executes if the condition is true.");
} else {
  console.log("This code executes if the condition is false.");
}
```

8.
 Understand what nesting is:
```
var outerCondition = true;
var innerCondition = false;

if (outerCondition) {
  console.log("Outer condition is true.");

  if (innerCondition) {
    console.log("Inner condition is true.");
  }
}

```

9.
Understand what truthy and falsy values are:
```
var truthyExample = "Hello"; // truthy
var falsyExample = 0;        // falsy

if (truthyExample) {
  console.log("Truthy example is true in a boolean context.");
}

if (!falsyExample) {
  console.log("Falsy example is false in a boolean context.");
}
```

___

1. What are the eight data types in JavaScript?
Number, String, Boolean, Undefined, Null, Object, Array, Symbol.

2. Which data type is NOT primitive?
Object is not a primitive data type.

3. What is the relationship between null and undefined?
Both represent the absence of a value, but they are used in slightly different contexts. undefined is usually the default value of a variable, while null is often assigned by developers to signify an intentional absence of a value.

4. What is the difference between single, double, and backtick quotes for strings?
Single and double quotes are interchangeable for creating strings. Backtick quotes allow for string interpolation and the embedding of variables/expressions.

5. What is the term for joining strings together?
Concatenation is the term for joining strings together.

6. Which type of quote lets you embed variables/expressions in a string?
Backtick (`) quotes (Template Literals) let you embed variables/expressions in a string.

7. How do you embed variables/expressions in a string?
Use backticks and ${} inside the string to embed variables/expressions.

8. How do you use escape characters in a string?
Use a backslash () before a character to escape it in a string.
```
var escapedString = "This is an example with a \"quoted\" word.";

```
9. What is the difference between the slice/substring/substr string methods?
slice(start, end): Extracts a portion of a string between start and end.
substring(start, end): Similar to slice but doesn't support negative indices.
substr(start, length): Extracts a specified number of characters from a string starting at the specified index.

10. What are the three logical operators, and what do they stand for?
&& (Logical AND), || (Logical OR), ! (Logical NOT).

11. What are the comparison operators?
==, ===, !=, !==, <, >, <=, >=.

12. What are truthy and falsy values?
Truthy values are values that evaluate to true in a boolean context. Falsy values are values that evaluate to false.

13. What are the falsy values in JavaScript?
false, 0, "" (empty string), null, undefined, NaN.

14. What are conditionals?
Conditionals are statements that execute different code based on specified conditions.

15. What is the syntax for an if/else conditional?
```
if (condition) {
  // Code to execute if the condition is true
} else {
  // Code to execute if the condition is false
}

```

16. What is the syntax for a switch statement?
```
switch (expression) {
  case value1:
    // Code to execute if expression equals value1
    break;
  case value2:
    // Code to execute if expression equals value2
    break;
  // ... additional cases
  default:
    // Code to execute if expression doesn't match any case
}
```

17. What is the syntax for a ternary operator?
```
var result = condition ? trueValue : falseValue;
```
18. What is nesting?
Nesting involves placing statements or structures within others, creating a hierarchical structure. For example, nesting if statements within other if statements or nesting loops.

Example:
```
var isRaining = true;
var hasUmbrella = false;
var isSunny = true;

if (isRaining) {
  console.log("It's raining!");

  if (hasUmbrella) {
    console.log("I have an umbrella. I'll stay dry.");
  } else {
    console.log("I don't have an umbrella. I'll get wet.");
  }

} else if (isSunny) {
  console.log("It's sunny!");

} else {
  console.log("It's neither raining nor sunny.");
}

```
In this example:
The outer conditional checks if it's raining.
If it's raining, the inner conditional checks if there's an umbrella.
If there's an umbrella, a message is logged about staying dry.
If there's no umbrella, a message is logged about getting wet.
If it's not raining, the code checks if it's sunny.
If it's neither raining nor sunny, a default message is logged.

This demonstrates the concept of nesting, where the inner conditional statements are nested within the outer conditional statement to create a more complex decision-making structure.