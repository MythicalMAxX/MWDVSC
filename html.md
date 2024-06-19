## 1. Introduction to HTML
### 1.1 What is HTML?
HTML (HyperText Markup Language) is the standard language for creating web pages and web applications. It describes the structure of a webpage using markup.

### 1.2 Why Learn HTML?
- Fundamental building block of web development.
- Easy to learn and widely used.
- Essential for creating structured content on the web.

## 2. Basic Structure of an HTML Document
### 2.1 HTML Document Structure
An HTML document consists of a series of elements. Here is the basic structure:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Page Title</title>
</head>
<body>
    <h1>This is a Heading</h1>
    <p>This is a paragraph.</p>
</body>
</html>
```

### 2.2 Explanation of the Structure
- `<!DOCTYPE html>`: Declares the document type and version of HTML.
- `<html>`: Root element of an HTML page.
- `<head>`: Contains meta-information about the document.
- `<title>`: Sets the title of the document.
- `<body>`: Contains the content of the document.

## 3. Common HTML Elements
### 3.1 Headings
HTML headings are defined with the `<h1>` to `<h6>` tags:
```html
<h1>This is a Heading 1</h1>
<h2>This is a Heading 2</h2>
<h3>This is a Heading 3</h3>
```

### 3.2 Paragraphs
Paragraphs are defined with the `<p>` tag:
```html
<p>This is a paragraph.</p>
```

### 3.3 Links
Links are created using the `<a>` tag:
```html
<a href="https://www.example.com">This is a link</a>
```

### 3.4 Images
Images are embedded using the `<img>` tag:
```html
<img src="image.jpg" alt="Description of Image">
```

## 4. HTML Attributes
### 4.1 What are Attributes?
Attributes provide additional information about HTML elements. They are always included in the opening tag and usually come in name/value pairs like this: `name="value"`.

### 4.2 Common Attributes
- `href` in `<a>`: Specifies the URL of the page the link goes to.
- `src` in `<img>`: Specifies the path to the image.
- `alt` in `<img>`: Provides alternative text for the image.

## 5. Lists in HTML
### 5.1 Ordered Lists
Ordered lists are created with the `<ol>` tag, and each list item is defined with the `<li>` tag:
```html
<ol>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ol>
```

### 5.2 Unordered Lists
Unordered lists are created with the `<ul>` tag, and each list item is defined with the `<li>` tag:
```html
<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>
```

## 6. Forms in HTML
### 6.1 Basic Form Structure
Forms are used to collect user input. The `<form>` element contains form controls such as text fields, checkboxes, and submit buttons:
```html
<form action="/submit-form" method="post">
    <label for="name">Name:</label><br>
    <input type="text" id="name" name="name"><br>
    <input type="submit" value="Submit">
</form>
```

### 6.2 Common Form Elements
- `<input>`: Defines an input control.
- `<label>`: Defines a label for an `<input>` element.
- `<textarea>`: Defines a multi-line text input control.
- `<button>`: Defines a clickable button.

## 7. Tables in HTML
### 7.1 Basic Table Structure
Tables are defined with the `<table>` tag. A table is divided into rows (`<tr>`), and each row is divided into cells (`<td>`):
```html
<table>
    <tr>
        <th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>Data 1</td>
        <td>Data 2</td>
    </tr>
</table>
```

### 7.2 Table Elements
- `<table>`: Defines a table.
- `<tr>`: Defines a table row.
- `<td>`: Defines a table cell.
- `<th>`: Defines a table header cell.

## 8. Semantic HTML
### 8.1 What is Semantic HTML?
Semantic HTML introduces meaning to the web page rather than just presentation. For example, `<header>`, `<footer>`, `<article>`, and `<section>` tags are semantic elements.

### 8.2 Importance of Semantic HTML
- Improves accessibility.
- Enhances SEO.
- Provides better code readability and maintainability.

### 8.3 Common Semantic Elements
- `<header>`: Represents the header of a section or page.
- `<nav>`: Contains navigation links.
- `<main>`: Represents the main content of the document.
- `<section>`: Defines a section in a document.
- `<article>`: Represents an independent piece of content.
- `<footer>`: Represents the footer of a section or page.

## 9. HTML5 Features
### 9.1 New Elements in HTML5
HTML5 introduced several new elements to enhance the web development experience:
- `<article>`
- `<section>`
- `<nav>`
- `<header>`
- `<footer>`
- `<figure>`
- `<figcaption>`
- `<aside>`

### 9.2 Multimedia Elements
HTML5 also brought new multimedia elements:
- `<audio>`: For embedding audio files.
- `<video>`: For embedding video files.
- `<canvas>`: For drawing graphics on the fly via scripting (usually JavaScript).

### 9.3 Forms Enhancements
HTML5 improved forms with new input types such as `email`, `date`, `url`, `range`, and more.

## 10. Best Practices in HTML
### 10.1 Clean and Readable Code
- Use proper indentation.
- Write comments to explain sections of your code.
- Use meaningful names for classes and IDs.

### 10.2 Accessibility
- Use semantic HTML elements.
- Provide alternative text for images.
- Ensure your site can be navigated using a keyboard.

### 10.3 SEO Optimization
- Use proper heading hierarchy.
- Use meta tags appropriately.
- Ensure your site is mobile-friendly.
