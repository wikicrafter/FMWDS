1. What is the difference between a block element and an inline element?
Block Element:
* Takes up the full width available.
* Starts on a new line.
* Examples: ```<div>, <p>, <h1>.```

    Inline Element:
* Takes only as much width as necessary.
* Does not start on a new line.
* Examples: ```<span>, <a>, <strong>.```


2. What is the difference between an inline element and an inline-block element?
Inline Element:
Does not allow setting width and height.
Ignores top and bottom margins/paddings.

    Inline-Block Element:
Allows setting width and height.
Respects top and bottom margins/paddings.
Example:
```
/* Example of inline-block */
.inline-block {
  display: inline-block;
  width: 100px;
  height: 50px;
  margin: 10px;
  background-color: lightblue;
}

```

3. Is an h1 block or inline?
```<h1>``` is a block-level element.

4. Is button block or inline?
```<button>``` is an inline-level element by default, but its display can be changed to block or inline-block using CSS.

5. Is div block or inline?
```<div>``` is a block-level element.

6. Is span block or inline?
```<span>``` is an inline-level element.