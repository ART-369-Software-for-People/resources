# HTML Basics

## Overview

- HTML stands for Hyper Text Markup Language.
- HTML is the standard markup language for creating Web pages
- HTML is not a programming language. It is a markup language that defines the structure of your content.
- HTML elements are the building blocks of HTML pages
- HTML elements are represented by tags, written using angle brackets: `<tagname>`, and in most cases, they are paired with a closing tag: `</tagname>`.
- HTML tags label pieces of content such as "heading", "paragraph", "table", and so on
- Browsers do not display the HTML tags, but use them to render the content of the page
- HTML tags can contain attributes. Attributes provide additional information about the element

## Basic HTML Document Structure

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width" />
    <title>Page Title</title>
</head>
<body>

<h1>This is a Heading</h1>
<p>This is a paragraph.</p>
<img src="link" alt="image" />

</body>
</html>
```

In the above example we have the following elements:

- `<!DOCTYPE html>`: declaration defines this document to be HTML5
- `<html>`: root element of the HTML page
- `<head>`: contains meta information about the document
- `<meta charset="utf-8" />`: specifies the character encoding for the HTML document
- `<meta name="viewport" content="width=device-width" />`: specifies how the page should be displayed on a device
- `<title>`: specifies a title for the document
- `<body>`: contains the visible page content
- `<h1>`: defines a large heading
- `<p>`: defines a paragraph
- `<img>`: defines an image
- `src`: specifies the URL of the image
- `alt`: specifies an alternate text for the image


## Nesting Elements

HTML elements can be nested (elements can contain elements). All HTML documents consist of nested elements. In this example, we would use a `<ul>` element to create a list of items. `<ul>` stands for unordered list and within the `<ul>` element, we would nest `<li>` elements, which stands for list items, to create a list of items.

```html
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>
```

## HTML Attributes

HTML elements can have attributes. Attributes provide additional information about the element. In this example, we would use the `id` attribute to give the `<h1>` element an identifier. The `id` attribute is used to uniquely identify an element in an HTML document.

```html
<h1 id="heading">This is a Heading</h1>
```
