In CSS, there are two main axes used in layout: the main axis and the cross axis.

Main Axis:
Definition: The main axis is the primary axis along which flex items or grid items are laid out. It is defined by the flex-direction property in Flexbox and the grid-template-rows or grid-template-columns properties in Grid.
Direction: The direction can be horizontal (left to right or right to left) or vertical (top to bottom or bottom to top), depending on the layout mode.

```
/* Example of main axis in Flexbox */
.flex-container {
  display: flex;
  flex-direction: row; /* Main axis is horizontal (left to right) */
}

```

```
/* Example of main axis in Grid */
.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr; /* Main axis is horizontal */
}
```


Cross Axis:
Definition: The cross axis is perpendicular to the main axis. In Flexbox, it is the axis along which flex items are aligned when align-items or align-self is used. In Grid, it is the axis perpendicular to the one specified by grid-template-rows or grid-template-columns.
Direction: It is perpendicular to the main axis.

```
/* Example of cross axis in Flexbox */
.flex-container {
  display: flex;
  align-items: center; /* Cross axis alignment */
}
```

```
/* Example of cross axis in Grid */
.grid-container {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  align-items: center; /* Cross axis alignment */
}
```

Understanding and manipulating these axes is crucial for creating flexible and responsive layouts in CSS. The main axis determines the primary direction of your layout, while the cross axis provides additional alignment options perpendicular to the main axis.


___

How do you make flex items arrange themselves vertically instead of horizontally?
Use flex-direction: column; to set the main axis to be vertical. By default, it is set to row, which arranges items horizontally.

```
.flex-container {
  display: flex;
  flex-direction: column; /* Items arrange vertically */
}
```

In a column flex-container, what does flex-basis refer to?
In a column flex-container, flex-basis sets the initial size of the flex items along the cross axis (vertical axis).

```
.flex-container {
  display: flex;
  flex-direction: column;
}

.flex-item {
  flex-basis: 50px; /* Initial height of the item in a column layout */
}
```

In a row flex-container, what does flex-basis refer to?
In a row flex-container, flex-basis sets the initial size of the flex items along the main axis (horizontal axis).

```
.flex-container {
  display: flex;
  flex-basis: 50px; /* Initial width of the item in a row layout */
}
```
Why do the previous two questions have different answers?
The main and cross axes are swapped when the flex-direction property is changed. In a column flex-container, the main axis is vertical, so flex-basis refers to the initial size along the vertical axis. In a row flex-container, the main axis is horizontal, so flex-basis refers to the initial size along the horizontal axis. The directionality of the layout determines the interpretation of flex-basis.