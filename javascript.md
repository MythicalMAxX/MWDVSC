## 1. Introduction to JavaScript
### 1.1 What is JavaScript?
JavaScript is a high-level, interpreted programming language that enables interactive web pages. It is an essential part of web development, allowing developers to create dynamic content and control multimedia.

### 1.2 Why Learn JavaScript?
- Adds interactivity to web pages.
- Enables client-side scripting.
- Widely used and supported across all browsers.

## 2. Basic Syntax of JavaScript
### 2.1 JavaScript Syntax
JavaScript is written in plain text and executed by the browser. A basic JavaScript statement ends with a semicolon:
```javascript
let message = "Hello, World!";
console.log(message);
```

### 2.2 Example
```javascript
let name = "Alice";
alert("Hello, " + name + "!");
```

## 3. How to Add JavaScript to HTML
### 3.1 Inline JavaScript
Inline JavaScript is included directly within HTML elements using the `onclick` attribute:
```html
<button onclick="alert('Button clicked!')">Click Me</button>
```

### 3.2 Internal JavaScript
Internal JavaScript is written within the `<script>` tag in the `<head>` or `<body>` section of an HTML document:
```html
<!DOCTYPE html>
<html>
<head>
    <script>
        function showMessage() {
            alert("Hello, World!");
        }
    </script>
</head>
<body>
    <button onclick="showMessage()">Click Me</button>
</body>
</html>
```

### 3.3 External JavaScript
External JavaScript is written in a separate `.js` file and linked to the HTML document:
```html
<!DOCTYPE html>
<html>
<head>
    <script src="script.js"></script>
</head>
<body>
    <button onclick="showMessage()">Click Me</button>
</body>
</html>
```
**script.js**
```javascript
function showMessage() {
    alert("Hello, World!");
}
```

## 4. Variables and Data Types
### 4.1 Declaring Variables
Variables store data values and are declared using `let`, `const`, or `var`:
```javascript
let x = 10;
const pi = 3.14;
var name = "Alice";
```

### 4.2 Data Types
JavaScript supports various data types including:
- **String**: Represents text.
  ```javascript
  let message = "Hello, World!";
  ```
- **Number**: Represents numerical values.
  ```javascript
  let count = 42;
  ```
- **Boolean**: Represents `true` or `false`.
  ```javascript
  let isActive = true;
  ```
- **Array**: Represents a collection of values.
  ```javascript
  let colors = ["red", "green", "blue"];
  ```
- **Object**: Represents an instance of a class.
  ```javascript
  let person = {firstName: "Alice", lastName: "Doe"};
  ```

## 5. Operators and Expressions
### 5.1 Arithmetic Operators
JavaScript supports basic arithmetic operators:
```javascript
let sum = 10 + 5;
let difference = 10 - 5;
let product = 10 * 5;
let quotient = 10 / 5;
```

### 5.2 Comparison Operators
Used to compare values and return a Boolean result:
```javascript
let isEqual = (10 == 5); // false
let isNotEqual = (10 != 5); // true
let isGreater = (10 > 5); // true
let isLess = (10 < 5); // false
```

### 5.3 Logical Operators
Used to combine Boolean values:
```javascript
let andResult = (true && false); // false
let orResult = (true || false); // true
let notResult = !true; // false
```

## 6. Functions
### 6.1 Defining Functions
Functions are blocks of code designed to perform a particular task. They are defined using the `function` keyword:
```javascript
function greet(name) {
    return "Hello, " + name + "!";
}
```

### 6.2 Calling Functions
Functions are executed when they are called:
```javascript
let message = greet("Alice");
alert(message); // "Hello, Alice!"
```

## 7. Events
### 7.1 Event Handling
Events are actions that can be detected by JavaScript. Common events include clicks, mouse movements, and key presses:
```javascript
<button onclick="displayDate()">Click me to display Date and Time.</button>
<script>
function displayDate() {
    document.getElementById("demo").innerHTML = Date();
}
</script>
```

### 7.2 Common Event Types
- **onclick**: Triggered when an element is clicked.
  ```html
  <button onclick="alert('Button clicked!')">Click Me</button>
  ```
- **onmouseover**: Triggered when the mouse pointer is moved over an element.
  ```html
  <div onmouseover="this.style.backgroundColor='yellow'">Hover over me!</div>
  ```

## 8. DOM Manipulation
### 8.1 What is the DOM?
The Document Object Model (DOM) is a programming interface for HTML documents. It represents the page so that programs can change the document structure, style, and content.

### 8.2 Selecting Elements
JavaScript provides several methods to select HTML elements:
- **getElementById**: Selects an element by its ID.
  ```javascript
  let element = document.getElementById("demo");
  ```
- **getElementsByClassName**: Selects elements by their class name.
  ```javascript
  let elements = document.getElementsByClassName("demo");
  ```
- **querySelector**: Selects the first element that matches a CSS selector.
  ```javascript
  let element = document.querySelector(".demo");
  ```

### 8.3 Modifying Elements
JavaScript can change the content and style of HTML elements:
- **Changing Content**:
  ```javascript
  document.getElementById("demo").innerHTML = "Hello, World!";
  ```
- **Changing Style**:
  ```javascript
  document.getElementById("demo").style.color = "red";
  ```

## 9. Loops and Conditional Statements
### 9.1 Conditional Statements
Conditional statements are used to perform different actions based on different conditions:
- **if Statement**:
  ```javascript
  let hour = 10;
  if (hour < 12) {
      alert("Good morning!");
  }
  ```
- **if...else Statement**:
  ```javascript
  let hour = 14;
  if (hour < 12) {
      alert("Good morning!");
  } else {
      alert("Good afternoon!");
  }
  ```

### 9.2 Loops
Loops are used to perform repeated tasks based on a condition:
- **for Loop**:
  ```javascript
  for (let i = 0; i < 5; i++) {
      console.log(i);
  }
  ```
- **while Loop**:
  ```javascript
  let i = 0;
  while (i < 5) {
      console.log(i);
      i++;
  }
  ```

## 10. JavaScript Best Practices
### 10.1 Writing Clean Code
- Use meaningful variable names.
- Keep code DRY (Don't Repeat Yourself).
- Comment your code to explain logic.

### 10.2 Debugging
- Use `console.log()` to print variables and messages to the console.
- Use the browser's developer tools to inspect elements and debug JavaScript code.
