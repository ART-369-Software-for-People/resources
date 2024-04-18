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

Other attributes include `class`, `style`, `href`, `src`, `alt`, and so on. Refer to the [HTML attributes reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes) for more information.

## Anchor Tag (Making Links)

The `<a>` tag serves as a hyperlink, allowing for navigation between pages. It can be seen as a gateway to other pages. The `href` attribute is the key attribute of the `<a>` element, specifying the destination of the link.

```html
<a href="https://alvinashiatey.com">Alvin Ashaitey</a>
```

### External Links

In the example above, the `href` attribute specifies an external link. External links link you to an external page, which is not on your website. They must include the full URL, including the protocol (e.g., `https://`).

### Internal Links

Internal links link you to another page on your website. They must include the relative path to the page you want to link to.

```html
<a href="about.html">About</a>
```

More information about external and internal links can be found [here](https://www.coffeecup.com/help/articles/absolute-vs-relative-pathslinks/).


## HTML Comments

HTML comments are not displayed in the browser. They are used to add notes to the code. Comments can be used to explain the code, or to prevent the browser from rendering specific parts of the code.

```html
<!-- This is a comment -->
<!-- °°°·.°·..·°¯°·._.· ART 369 ·._.·°¯°·.·° .·°°° -->
```

## Semantic HTML

- Semantic HTML is a way of writing HTML that emphasizes the meaning of the content rather than its appearance.
- In HTML, you can technically use any tag to create any layout you want. However, using the correct tags for the correct purpose is important for [accessibility](https://www.accessibility-developer-guide.com/knowledge/semantics/), and readability.
- While some tags may appear identical, they actually hold distinct connotations for screen readers. For instance, a `<div>` tag serves as a general container, whereas a `<header>` tag serves as a container for introductory content.

```html
<!-- Non-semantic HTML -->
<div id="header">
    <h1>My Website</h1>
</div>

<!-- Semantic HTML -->
<header>
    <h1>My Website</h1>
</header>
```

## File Structure

When creating an HTML file, it is important to have a well-organized file structure. This is especially important when working on larger projects. Below is an example of a simple file structure for an HTML project.

```tree
project-folder/
│
├── css/
│   └── style.css
│
├── img/
│   └── image.jpg
│
├── js/
│   └── script.js
│
├── index.html
```

In the example above, we have a project folder that contains a `css` folder for CSS files, an `img` folder for image files, a `js` folder for JavaScript files, and an `index.html` file for the main HTML content.