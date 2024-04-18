# CSS Layout

## Overview

- There are many ways to layout a webpage using CSS.
- The most common layout methods are:
  - Floats
  - Flexbox
  - Grid
- Each method has its own strengths and weaknesses.
- The best method to use depends on the layout you are trying to achieve.
- In this document, we will cover Flexbox and Grid.

## Flexbox

- Flexbox, short for the Flexible Box Layout Module
- Flexbox is a one-dimensional layout method.
- It is best used for laying out items in a row or a column.

### Flex Container

- To use Flexbox, you must first create a flex container.
- To create a flex container, set the display property of an element to `flex`.

```html
<div class="container">
  <!-- Flex items go here -->
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>
```

By default the above items will be laid out in a row.

<iframe width="100%" height="300" src="//jsfiddle.net/alvinashiatey/L60dwj5o/5/embedded/html,css,result/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>
