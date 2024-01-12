Lesson overview
This section contains a general overview of topics that you will learn in this lesson.
Creating objects.
Accessing object properties.
Being able to use multiple object operators.
Being able to use some powerful array functions.

### Creating Objects:
In JavaScript, you can create objects using either object literals or the Object constructor. Object literals are more commonly used for simplicity.
```
// Object Literal
const person = {
  firstName: 'John',
  lastName: 'Doe',
  age: 30,
  address: {
    city: 'New York',
    country: 'USA'
  },
  sayHello: function() {
    console.log(`Hello, my name is ${this.firstName} ${this.lastName}`);
  }
};

// Accessing Object Properties
console.log(person.firstName); // Output: John
console.log(person.address.city); // Output: New York

// Invoking Object Method
person.sayHello(); // Output: Hello, my name is John Doe
```

### Accessing Object Properties:
You can access object properties using dot notation or square brackets.
Example using Dot Notation:
```
const car = {
  make: 'Toyota',
  model: 'Camry',
  year: 2022
};

console.log(car.make); // Output: Toyota
console.log(car['model']); // Output: Camry
```

### Using Multiple Object Operators:
Combining multiple object operators allows you to navigate through nested objects or access properties dynamically.
Example using Multiple Operators:
```
const company = {
  name: 'TechCo',
  departments: {
    development: {
      teamLead: 'Alice',
      engineers: ['Bob', 'Charlie']
    },
    marketing: {
      manager: 'Eve',
      designers: ['Frank', 'Grace']
    }
  }
};

console.log(company.departments.development.teamLead); // Output: Alice
const department = 'marketing';
console.log(company.departments[department].manager); // Output: Eve
```

### Using Powerful Array Functions:
JavaScript provides powerful array functions like map, filter, and reduce that can be used with array
Example:
```
const numbers = [1, 2, 3, 4, 5];

// Map: doubling each number
const doubledNumbers = numbers.map(num => num * 2);
console.log(doubledNumbers); // Output: [2, 4, 6, 8, 10]

// Filter: keeping only even numbers
const evenNumbers = numbers.filter(num => num % 2 === 0);
console.log(evenNumbers); // Output: [2, 4]

// Reduce: summing all numbers
const sum = numbers.reduce((acc, num) => acc + num, 0);
console.log(sum); // Output: 15
```

These examples showcase the creation of objects, accessing their properties, using multiple object operators, and leveraging powerful array functions in JavaScript.

___

### Difference between Objects and Arrays:
Objects: Objects are collections of key-value pairs, where each key is a string (or symbol) and each value can be any data type. Objects are used to represent entities with properties.
```
const person = {
  name: 'John',
  age: 25,
  city: 'New York'
};
```

Arrays: Arrays are ordered lists of values. Each value in an array is associated with an index, starting from zero. Arrays are used to store and manipulate ordered collections of data.

```
const numbers = [1, 2, 3, 4, 5];
```


### Accessing Object Properties:
Object properties can be accessed using dot notation or square bracket notation.
```
const person = {
  name: 'John',
  age: 25,
  city: 'New York'
};

console.log(person.name); // Output: John
console.log(person['age']); // Output: 25
```


### Array.prototype.map():
Array.prototype.map() is a method in JavaScript that creates a new array by applying a provided function to each element of the original array. It returns a new array without modifying the original array.
```
const numbers = [1, 2, 3, 4, 5];

const doubledNumbers = numbers.map(num => num * 2);
console.log(doubledNumbers); // Output: [2, 4, 6, 8, 10]
```

### Array.prototype.reduce():
Array.prototype.reduce() is a method in JavaScript that reduces an array to a single value by applying a provided function to each element and accumulating the results. It is often used for tasks such as summing or calculating averages.
```
const numbers = [1, 2, 3, 4, 5];

const sum = numbers.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
console.log(sum); // Output: 15
```
In summary, objects and arrays serve different purposes: objects for key-value pairs, and arrays for ordered lists. Accessing object properties involves dot or bracket notation. Array.prototype.map() is useful for transforming array elements, while Array.prototype.reduce() is useful for aggregating array elements into a single value.