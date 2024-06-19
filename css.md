## 1. Introduction to CSS
### 1.1 What is CSS?
CSS (Cascading Style Sheets) is a stylesheet language used to describe the presentation of an HTML document. CSS controls the layout, colors, fonts, and overall look and feel of a webpage.

### 1.2 Why Learn CSS?
- Separates content from design.
- Enables flexible and responsive design.
- Enhances user experience.

## 2. Basic Syntax of CSS
### 2.1 CSS Syntax
A CSS rule consists of a selector and a declaration block:
```css
selector {
    property: value;
}
```

### 2.2 Example
```css
p {
    color: blue;
    font-size: 16px;
}
```
- `p`: Selector, targets all `<p>` elements.
- `color: blue;`: Declaration, sets the text color to blue.
- `font-size: 16px;`: Declaration, sets the font size to 16 pixels.

## 3. How to Add CSS to HTML
### 3.1 Inline CSS
Inline CSS uses the `style` attribute inside HTML elements:
```html
<p style="color: blue;">This is a blue paragraph.</p>
```

### 3.2 Internal CSS
Internal CSS is defined within a `<style>` tag in the `<head>` section of an HTML document:
```html
<!DOCTYPE html>
<html>
<head>
    <style>
        p {
            color: blue;
        }
    </style>
</head>
<body>
    <p>This is a blue paragraph.</p>
</body>
</html>
```

### 3.3 External CSS
External CSS is defined in a separate `.css` file linked to the HTML document:
```html
<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" type="text/css" href="styles.css">
</head>
<body>
    <p>This is a blue paragraph.</p>
</body>
</html>
```
**styles.css**
```css
p {
    color: blue;
}
```

## 4. Selectors in CSS
### 4.1 Types of Selectors
- **Element Selector**: Targets HTML elements.
  ```css
  p {
      color: red;
  }
  ```
- **Class Selector**: Targets elements with a specific class attribute.
  ```css
  .className {
      color: green;
  }
  ```
- **ID Selector**: Targets a single element with a specific ID attribute.
  ```css
  #idName {
      color: blue;
  }
  ```
- **Attribute Selector**: Targets elements with a specific attribute.
  ```css
  [type="text"] {
      border: 1px solid black;
  }
  ```

## 5. CSS Box Model
### 5.1 Understanding the Box Model
The CSS box model describes the rectangular boxes generated for elements in the document tree and consists of margins, borders, padding, and the content area.
- **Content**: The innermost part where text and images appear.
- **Padding**: Clears an area around the content (inside the border).
- **Border**: A border surrounding the padding (and content).
- **Margin**: Clears an area outside the border.

### 5.2 Example
```css
div {
    width: 300px;
    padding: 20px;
    border: 5px solid black;
    margin: 15px;
}
```

## 6. Styling Text
### 6.1 Font Properties
- **font-family**: Specifies the font of the text.
  ```css
  p {
      font-family: Arial, sans-serif;
  }
  ```
- **font-size**: Specifies the size of the text.
  ```css
  p {
      font-size: 16px;
  }
  ```
- **font-weight**: Specifies the weight (boldness) of the text.
  ```css
  p {
      font-weight: bold;
  }
  ```

### 6.2 Text Properties
- **color**: Specifies the color of the text.
  ```css
  p {
      color: red;
  }
  ```
- **text-align**: Specifies the horizontal alignment of the text.
  ```css
  p {
      text-align: center;
  }
  ```
- **text-decoration**: Adds decoration to text (underline, overline, line-through).
  ```css
  p {
      text-decoration: underline;
  }
  ```

## 7. Styling Backgrounds
### 7.1 Background Color
Sets the background color of an element:
```css
body {
    background-color: lightblue;
}
```

### 7.2 Background Image
Sets a background image for an element:
```css
body {
    background-image: url('background.jpg');
}
```

### 7.3 Background Properties
- **background-repeat**: Controls the repetition of the background image.
  ```css
  body {
      background-repeat: no-repeat;
  }
  ```
- **background-size**: Controls the size of the background image.
  ```css
  body {
      background-size: cover;
  }
  ```

## 8. Layout with CSS
### 8.1 Display Property
Controls the display behavior of an element:
```css
div {
    display: none; /* Hides the element */
}
```
- **block**: Displays an element as a block.
- **inline**: Displays an element as an inline element.
- **none**: Hides the element.

### 8.2 Position Property
Specifies the type of positioning method used for an element:
```css
div {
    position: relative;
    top: 10px;
    left: 20px;
}
```
- **static**: Default position.
- **relative**: Positioned relative to its normal position.
- **absolute**: Positioned relative to the nearest positioned ancestor.
- **fixed**: Positioned relative to the browser window.
- **sticky**: Toggles between relative and fixed, depending on the scroll position.

### 8.3 Flexbox
A layout model that provides a more efficient way to lay out, align, and distribute space among items in a container:
```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
}
```
- **justify-content**: Aligns items horizontally.
- **align-items**: Aligns items vertically.

### 8.4 Grid
A layout system for creating complex and responsive grid-based layouts:
```css
.container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
}
```
- **grid-template-columns**: Defines the columns of the grid.
- **gap**: Defines the spacing between grid items.

## 9. Responsive Design
### 9.1 Media Queries
Used to apply different styles for different devices or screen sizes:
```css
@media (max-width: 600px) {
    body {
        background-color: lightgreen;
    }
}
```

### 9.2 Responsive Units
- **Percentage**: Relative to the parent element.
  ```css
  div {
      width: 50%;
  }
  ```
- **Viewport Units**: Relative to the viewport dimensions.
  ```css
  div {
      width: 50vw; /* 50% of the viewport width */
  }
  ```

## 10. CSS Frameworks
### 10.1 Introduction to CSS Frameworks
CSS frameworks provide pre-written CSS that helps in designing web pages quickly:
- **Bootstrap**
- **Tailwind CSS**
- **Bulma**

### 10.2 Benefits of Using CSS Frameworks
- Speeds up development.
- Ensures a consistent design.
- Provides responsive design out of the box.