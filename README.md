# Master JavaScript Interview Preparation: Essential Concepts, Tips, and Practice Questions

Looking to ace your next JavaScript interview? This blog covers everything you need to know! Whether you're a beginner or an experienced developer, we dive into core concepts like closures, promises, event loop, and async/await, along with coding patterns, common mistakes, and best practices. With a curated set of practice questions and detailed explanations, you'll feel confident and ready to tackle any JavaScript interview. Level up your knowledge and land your dream job!

### Table of Contents

| No. | Questions |
| --- | --------- |
| 1 | [What is JavaScript?](#1-what-is-javascript) |
| 2 | [What are the data types in JavaScript?](#2-what-are-the-data-types-in-javascript) |
| 3 | [Difference between `==` and `===`](#3-difference-between--and-) |


### 1. What is JavaScript?

JavaScript is a high-level, interpreted programming language primarily used to create interactive and dynamic web pages. It is part of the three core web technologies: HTML, CSS, and JavaScript. While HTML and CSS are responsible for structure and styling, JavaScript handles the behavior of a website. JavaScript can also be used in server-side development (with Node.js), mobile applications, and more.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>JavaScript Example</title>
</head>
<body>
    <h1 id="heading">Hello, World!</h1>
    <button onclick="changeText()">Click me!</button>

    <script>
        function changeText() {
            document.getElementById('heading').innerText = 'You clicked the button!';
        }
    </script>
</body>
</html>
```
Here, clicking the button changes the text of the `<h1>` element using JavaScript.

**[⬆ Back to Top](#table-of-contents)**


### 2. What are the data types in JavaScript?

JavaScript has several data types, including:

- **Primitive types:** These types are immutable.
    - ***String:*** Represents textual data.
    - ***Number:*** Represents numbers (both integers and floating-point).
    - ***Boolean:*** Represents true or false values.
    - ***Null:*** Represents an intentional absence of any object value.
    - ***Undefined:*** Represents a variable that has been declared but not assigned a value.
    - ***Symbol:*** Introduced in ES6, used to create unique identifiers.
    - ***BigInt:*** Introduced in ES2020, used for very large integers.

- **Non-primitive types:** Objects, Arrays, Functions.

```
let str = "Hello";  // String
let num = 42;       // Number
let bool = true;    // Boolean
let undef;          // Undefined
let empty = null;   // Null
let symbol = Symbol('unique'); // Symbol
let bigInt = 9007199254740991n; // BigInt
```

**[⬆ Back to Top](#table-of-contents)**

### 3. Difference between `==` and `===`?

- **== (Abstract Equality):** Compares two values after performing type conversion if they are of different types.

- **=== (Strict Equality):** Compares both value and type without converting the types.

```
console.log(5 == '5');  // true (because '5' is type-converted to number 5)
console.log(5 === '5'); // false (because '5' is a string and 5 is a number)
```

In general, it’s better to use `===` to avoid unexpected type coercion.

**[⬆ Back to Top](#table-of-contents)**

### 4. What is a variable?

A variable in JavaScript is a container that holds a value. You can declare a variable using `var`, `let`, or `const`.

- **var:** The oldest way to declare variables, scoped to the function or globally, and can be redeclared and updated.

- **let:** Introduced in ES6, it's block-scoped and can be updated but not redeclared in the same scope.

- **const:** Also block-scoped but cannot be updated or redeclared once assigned.

```
var name = "John";   // Global or function scope
let age = 30;        // Block scope (within a specific block)
const country = "USA"; // Block scope, cannot be reassigned
```

**[⬆ Back to Top](#table-of-contents)**
