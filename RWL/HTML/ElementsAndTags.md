##  What is an HTML Elements and Tag? 

In HTML (Hypertext Markup Language), elements are the building blocks of a web page. An HTML document is composed of a series of elements, each represented by tags. Tags define the structure and content of the document, and they are written using angle brackets < >. Here's a brief overview of HTML elements and tags:

Element Structure:

An HTML element consists of an opening tag, content, and a closing tag.
Opening Tag: ```<tagname>```
Closing Tag: ```</tagname>```
Content: The actual content of the element goes between the opening and closing tags.

#### Common HTML Tags:

```<!DOCTYPE html>```: Specifies the HTML version being used (HTML5 in this case).
```<html>```: The root element that wraps all content on the page.
```<head>```: Contains meta-information about the HTML document, such as the title, character set, styles, etc.
```<title>```: Sets the title of the HTML document, which appears in the browser's title bar or tab.
```<body>```: Contains the main content of the HTML document.
```<h1>``` to ```<h6>```: Headings, with ```<h1>``` being the largest and ```<h6>``` the smallest.
```<p>```: Paragraph.
```<a>```: Anchor, used for hyperlinks.
```<img>```: Image.
```<ul>```: Unordered list.
```<ol>```: Ordered list.
```<li>```: List item.
```<div>```: Division or a container that helps structure the layout.
```<span>```: Inline container typically used for styling a specific piece of text.
Attributes:

HTML tags can have attributes that provide additional information about the element.
Attributes are added to the opening tag and are usually name-value pairs, like attribute="value".
Example: ```<a href="https://www.example.com">Visit Example</a>```

### Example
```
<!DOCTYPE html>
<html>
  <head>
    <title>My First HTML Page</title>
  </head>
  <body>
    <h1>Hello, World!</h1>
    <p>This is a paragraph.</p>
    <ul>
      <li>Item 1</li>
      <li>Item 2</li>
    </ul>
  </body>
</html>
```