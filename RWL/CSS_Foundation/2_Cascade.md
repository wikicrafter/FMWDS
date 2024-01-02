What the cascade does:
The cascade resolves conflicting styles by considering specificity, importance, and source order. Styles declared later or with higher specificity take precedence. 
Example:
```
p {
  color: blue; /* Style from a general rule */
}

.special {
  color: red; /* Style from a more specific rule */
}
```
___
Specificity and combining CSS selectors:
Specificity is determined by the type, class, and ID selectors. Combining selectors increases specificity. 
Example:
```
h1 {
  color: green; /* Less specific */
}

body h1 {
  color: orange; /* More specific due to the combination */
}

```

___
How inheritance affects certain properties:
Inheritance allows properties from a parent to be inherited by its children. 
Example:
```
body {
  font-family: Arial, sans-serif; /* Inherited font-family property */
  color: black;
}

p {
  /* Inherits font-family from the body */
  color: inherit; 
}

```
In this example, the p element inherits the font-family property from the body element.
___
Between a rule that uses one class selector and a rule that uses three type selectors, which rule has the higher specificity?

The specificity of a CSS rule is determined by the number and types of selectors it contains. In general, more specific selectors have higher specificity. Here's a breakdown of the specificity:

1. One Class Selector:
```
.example {
  color: blue;
}
```
Specificity: One class selector has a moderate specificity.

2. Three Type Selectors:
``` 
div p a {
  color: red;
}
```
Specificity: Three type selectors have a higher specificity compared to one class selector.
___
So, between a rule that uses one class selector and a rule that uses three type selectors, the rule with three type selectors has the higher specificity.




