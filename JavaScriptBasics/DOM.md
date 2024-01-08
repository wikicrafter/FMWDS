### 1. Explain what the DOM is in relation to a webpage:
Definition:
The Document Object Model (DOM) is a programming interface for web documents. It represents the structure of a webpage as a tree of objects, allowing scripts to dynamically update the content, structure, and style of a document.
Example:
```
<!DOCTYPE html>
<html>
  <head>
    <title>DOM Example</title>
  </head>
  <body>
    <h1>Hello, World!</h1>
    <p>This is a paragraph.</p>
  </body>
</html>
```
In this HTML document, the DOM represents each element (html, head, title, body, h1, p) as nodes in a tree structure.

### 2. Explain the difference between a “node” and an “element”:
Node vs. Element:
A node is a generic term for any object in the DOM tree, including elements, text, attributes, etc.
An element is a specific type of node that represents a tag in the HTML document.

### 3. Explain how to target nodes with “selectors”:
Selectors:
Selectors are patterns used to identify and target specific elements in the DOM.
Common selectors include tag names, class names, IDs, attribute values, etc.
Example: 
```
// Select by tag name
var paragraphs = document.getElementsByTagName("p");

// Select by class name
var highlighted = document.getElementsByClassName("highlight");

// Select by ID
var header = document.getElementById("main-header");
```

### 4. Explain the basic methods for finding/adding/removing and altering DOM nodes:

Basic Methods:
Finding:
getElementById, getElementsByClassName, getElementsByTagName, querySelector, querySelectorAll.


Adding:
createElement, appendChild, insertBefore.


Removing:
removeChild.

Altering:
Modifying properties like innerHTML, textContent, and attributes.

### 5. Explain the difference between a “nodelist” and an “array of nodes”:
NodeList vs. Array:
A NodeList is a collection of nodes returned by methods like getElementsByClassName or getElementsByTagName.
An Array of Nodes is a standard JavaScript array that can hold nodes. While they may seem similar, they have different available methods

### 6. Explain what “bubbling” is and how it works:
Bubbling:
Event bubbling is the propagation of events through the DOM tree from the target element up to the root.
When an event occurs on a nested element, it triggers the same event on its ancestors.
```
<div id="parent">
  <button id="child">Click me</button>
</div>

<script>
  document.getElementById("parent").addEventListener("click", function() {
    console.log("Parent clicked");
  });

  document.getElementById("child").addEventListener("click", function() {
    console.log("Child clicked");
  });
</script>
```

If you click the button, both "Child clicked" and "Parent clicked" will be logged, demonstrating event bubbling.

___

### 1. What is the DOM?
Definition:
The Document Object Model (DOM) is a programming interface that represents the structure of a document as a tree of objects. It provides a way for scripts to interact with the content, structure, and style of a webpage.

### 2. How do you target the nodes you want to work with

Targeting Nodes:
Use selectors to target nodes, such as getElementById, getElementsByClassName, getElementsByTagName, querySelector, and querySelectorAll.

### 3. How do you create an element in the DOM?
Creating Elements:
Use document.createElement to create a new element.
```
var newDiv = document.createElement("div");
```

### 4. How do you add an element to the DOM?
Adding Elements:
Use methods like appendChild or insertBefore to add elements to the DOM.
```
var parent = document.getElementById("parent");
parent.appendChild(newDiv);
```
### 5. How do you remove an element from the DOM?
Removing Elements:
Use removeChild to remove an element.
```
var child = document.getElementById("child");
parent.removeChild(child);
```

### 6. How can you alter an element in the DOM?
Altering Elements:
Modify properties and attributes of an element using innerHTML, textContent, and other DOM properties.

### 7. When adding text to a DOM element, should you use textContent or innerHTML? Why?

textContent vs. innerHTML:
Use textContent when dealing with text content to avoid potential security issues related to HTML injection.


### 8. Where should you include your JavaScript tag in your HTML file when working with DOM nodes?

Script Placement:
Generally, include the
 ```
 <script>
 ```
  tag at the end of the 
  ```
  <body>
  ```
   element to ensure that the DOM has been fully parsed before executing JavaScript.


### 9. How do “events” and “listeners” work?
Events and Listeners:
Events are interactions or occurrences in the browser (e.g., clicks, keypresses).
Listeners are functions that "listen" for events and execute code when the event occurs.


### 10. What are three ways to use events in your code?

Ways to Use Events:
Inline HTML event attributes (onclick, onmouseover).
DOM property events (element.onclick = function(){}).
Event listeners (element.addEventListener("click", function(){})).

### 11. Why are event listeners the preferred way to handle events?

Benefits of Event Listeners:
They allow attaching multiple listeners to one event.
They support capturing and bubbling phases.
They provide a cleaner separation of HTML and JavaScript.


### 12. What are the benefits of using named functions in your listeners?

Benefits of Named Functions:
Improved code readability and maintainability.
Easy removal of listeners using removeEventListener.


### 13. How do you attach listeners to groups of nodes?

Attaching Listeners to Groups:
Use a loop to iterate through a NodeList or an array of elements, attaching the listener to each.


### 14. What is the difference between the return values of querySelector and querySelectorAll?

Difference:
querySelector returns the first matching element.
querySelectorAll returns a NodeList containing all matching elements.

### 15. What does a “nodelist” contain?

NodeList Content:
A NodeList contains a collection of nodes, which can be elements, text nodes, attributes, etc.


### 16. Explain the difference between “capture” and “bubbling”.

Capture vs. Bubbling:
Capture is the first phase of event propagation, going from the root to the target.
Bubbling is the second phase, going from the target back up to the root.
Event listeners can be set to capture or bubble using the addEventListener method with the useCapture parameter.