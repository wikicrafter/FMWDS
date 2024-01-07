How do you declare a variable?
What are three different ways to declare a variable?
Which one should you use when?
What are the rules for naming variables?
What are operators, operands, and operations?
What is concatenation and what happens when you add numbers and strings together?
What are the different types of operators in JavaScript?
What is the difference between == and ===?
What are operator precedence values?
What are the increment/decrement operators?
What is the difference between prefixing and postfixing them?
What are assignment operators?
What is the Unary Plus Operator?

___
1. How do you declare a variable?
To declare a variable in JavaScript, use the var, let, or const keyword, followed by the variable name.
Example:

```
var myVariable;
let anotherVariable;
const constantVariable = 42;
```

2. What are three different ways to declare a variable?
Using var:

```
var x;
```

Using let:

```
let y;
```

Using const:

```
const z = 10;
```

3. Which one should you use when?
Use const for variables that won't be reassigned.
Use let for variables that may be reassigned.
Use var if you're dealing with older code or specific scenarios, but prefer let and const for modern JavaScript.

4. What are the rules for naming variables?
Variable names must start with a letter, underscore (_), or dollar sign ($).
Subsequent characters can also be numbers.
Avoid reserved words (e.g., let, const, function).
Follow camelCase or snake_case conventions for readability.

5.  What are operators, operands, and operations?
Operators: Symbols that perform operations on variables and values.
Operands: Values or variables that operators act upon.
Operations: Actions performed by operators.

6. What is concatenation, and what happens when you add numbers and strings together?
Concatenation: Joining strings together.
```
var firstName = "John";
var lastName = "Doe";
var fullName = firstName + " " + lastName; // Concatenation

```

When you add numbers and strings, JavaScript converts numbers to strings during concatenation.
```
var num = 42;
var str = "The answer is: " + num; // Conversion to string
```


7. What are the different types of operators in JavaScript?
Arithmetic Operators: +, -, *, /, %.
Comparison Operators: ==, ===, !=, !==, <, >, <=, >=.
Logical Operators: &&, ||, !.
Assignment Operators: =, +=, -=, *=, /=.
Unary Operators: ++, --, typeof, delete.


8. What is the difference between == and ===?
== performs type coercion, allowing different types to be considered equal.
=== strictly compares values without type coercion, ensuring both value and type match.

9. What are operator precedence values?
Operator precedence determines the order in which operators are executed.
Higher precedence values result in operators being evaluated first.

10. What are the increment/decrement operators?
Increment (++) increases a variable by 1.
Decrement (--) decreases a variable by 1.


11. What is the difference between prefixing and postfixing them?
Prefix (++x, --x): Increments/decrements the variable before its value is used.
Postfix (x++, x--): Uses the current value of the variable before incrementing/decrementing.


12. What are assignment operators?
Assignment operators assign values to variables.
```
var x = 5; // Assignment
x += 3;    // Increment and assign

```

13. What is the Unary Plus Operator?
The unary plus operator (+) attempts to convert its operand to a number.
```
var str = "42";
var num = +str; // Converts "42" to 42

```