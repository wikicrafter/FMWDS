
What is the syntax for class and ID selectors?
Class selector: ```.classname```
ID selector: ```#idname```
___
How would you apply a single rule to two different selectors?
Separate the selectors with a comma.
css
Code:
.selector1, #selector2 {
  /* CSS rule */
}
___
Given an element that has an id of title and a class of primary, how would you use both attributes for a single rule?
Combine them without spaces: #title.primary { /* CSS rule */ }
___
What does the descendant combinator do?
The descendant combinator ```(` `)``` selects all elements that are descendants of a specified element.
```
div p {
  /* CSS rule for paragraphs inside a div */
}   
```
___
What are the names of the three ways to add CSS to HTML?
Inline, Internal (in the head), and External (linked).
___
What are the main differences between the three ways of adding CSS to HTML?
Inline: Applied directly to an HTML element using the style attribute.
Internal: Placed within the ```<style>``` element in the HTML document's head.
External: Linked to the HTML document using the ```<link>``` element. External CSS is stored in a separate file.
Main differences include maintainability, reusability, and separation of concerns. Inline is specific to an element, internal is specific to a document, and external allows for a centralized stylesheet.
