# CSS Basics

## Overview

- CSS stands for Cascading Style Sheets.
- CSS describes how HTML elements are to be displayed on screen, paper, or in other media.
- There is a debate on whether CSS is a programming language or not. For the purpose of this course, CSS is not considered a programming language.

## Basic CSS Syntax

```css
selector {
    property: value;
}
```

In the above example we have the following elements:

- `selector`: selects the HTML element that you want to style
- `property`: specifies the style attribute you want to change
- `value`: specifies the value of the style attribute
- `property: value;`: Here we have the CSS declaration. The property and value pair are separated by a colon, and each declaration is separated by a semicolon.
- `selector { property: value; }`: the selector and property-value pair is enclosed in curly braces

## CSS Selectors

CSS selectors are used to "find" (or select) the HTML elements you want to style. Below are some more common CSS selectors:

- `element`: selects all elements of the specified type
- `.class`: selects all elements with the specified class name
- `#id`: selects an element with a specific id
- `[attribute]`: selects all elements with the specified attribute
- `[attribute=value]`: selects all elements with the specified attribute and value
- `:pseudo-class`: selects elements based on a certain state
- `::pseudo-element`: selects a certain part of an element

Here are some examples:

```css
/* Selects all <p> elements */
p {
    color: red;
    font-size: 20px;
    font-family: Arial;
}

/* Selects all elements with class="example" */
.example {
    color: blue;
}

/* Selects the element with id="example" */
#example {
    color: green;
}
```

In the above example, we selected the `<p>` element, elements with the class name `example`, and the element with the ID `example`. These selectors target single elements.

### Grouping Selectors

You can group selectors to apply the same styles to multiple elements. Here is an example:

```css
h1, h2, p {
    color: blue;
    font-family: Arial;
}
```

## CSS Properties

CSS properties are used to specify the style of an element. Breaking down the above example, we have the following properties:

- `color`: specifies the text color of an element
- `font-size`: specifies the font size of the text
- `font-family`: specifies the font family of the text

There are many CSS properties available. Refer to the [CSS reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference) for more information.
  
## Writing CSS

There are three ways to apply CSS to an HTML document:

1. **Inline CSS**: CSS is applied directly to the HTML element using the `style` attribute. This is not recommended as it mixes content with presentation.

```html
<p style="color: red;">This is a paragraph.</p>
```

2. **Internal CSS**: CSS is placed within the `<style>` element in the `<head>` section of the HTML document. This is recommended for small projects.

```html
<!DOCTYPE html>
<html>
<head>
    <style>
        p {
            color: red;
        }
    </style>
</head>
<body>
        <p>This is a paragraph.</p>
</body>
</html>
```

3. **External CSS**: CSS is placed in a separate file and linked to the HTML document using the `<link>` element. This is recommended for larger projects.

```html
<!DOCTYPE html>
<html>
<head>
        <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
        <p>This is a paragraph.</p>
</body>
</html>
```

``` css
/* styles.css */
p {
    color: red;
}
```

the file structure would look like this:

```
project-folder/
│
├── index.html
├── styles.css
```

## References and Resources

- [CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)
- [CSS Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics)
- [Getting to Know CSS by Shaw Howe](https://learn.shayhowe.com/html-css/getting-to-know-css/)
- [Basics of CSS by Laurel Schwulst](https://www.youtube.com/watch?v=BUZIaTHm_oE&feature=youtu.be)
