# read-class-02
## 1-Why is it important to use semantic elements in our HTML?
The semantic HTML tags help the search engines and other user devices to determine the importance and context of web pages. The pages made with semantic elements are much easier to read. It has greater accessibility. It offers a better user experience.
## 2-How many levels of headings are there in HTML?
There are six levels in the heading tag in HTML. They have decreasing order of importance/level starting from 1 to 6. Heading tags in HTML are used to give a title or subtitle to the section on the webpage.
                                               
<h1>Heading 1</h1>                                 
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>

## 3-What are some uses for the <sup> and <sub> elements?
### `<sub>`: The Subscript element
The `<sub>` HTML element specifies inline text which should be displayed as subscript for solely typographical reasons. Subscripts are typically rendered with a lowered baseline using smaller text.

```
<p>
  Almost every developer's favorite molecule is C<sub>8</sub>H<sub>10</sub>N<sub>4</sub>O<sub>2</sub>, also known as
  "caffeine."
</p>

```

### `<sup>:` The Superscript element
The `<sup>` HTML element specifies inline text which is to be displayed as superscript for solely typographical reasons. Superscripts are usually rendered with a raised baseline using smaller text.

```
<p>The <em>Pythagorean theorem</em> is often expressed as the following equation:</p>

```



## 4-When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?
- `<abbr>:` The Abbreviation element The <abbr> HTML element represents an abbreviation or acronym.

```html
<p>
  You can use <abbr>CSS</abbr> (Cascading Style Sheets) to style your <abbr>HTML</abbr> (HyperText Markup Language).
  Using style sheets, you can keep your <abbr>CSS</abbr> presentation layer and <abbr>HTML</abbr> content layer
  separate. This is called "separation of concerns."
 </p>
```

### Learn CSS
## 1-What are ways we can apply CSS to our HTML?
- **Inline Styles**
  Directly applied to individual HTML elements using the style attribute.
```
<p <strong>style</strong>="color: blue;">This is a blue text.</p>
```
 - **Internal Styles**
   Placed within the <style> tags in the <head> section of an HTML document.
  ```
 <head>
  <style>
    p {
      color: red;
    }
  </style>
</head>
<body>
  <p>This is a red text.</p>
</body>
```
- **External Styles**
CSS rules are placed in a separate .css file.
This file is then linked to the HTML document using the <link> tag.
```
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

## 2-Why should we avoid using inline styles?
The build-up of the inline CSS styles often translates into code duplication, making the project harder to maintain when the same style needs to be changed in several places. The same applies to the inline JavaScript snippets, as they cannot be reused across Screens or Web Blocks.

## 3-What is representing the selector?
In CSS, a selector is a pattern that matches specific elements in an HTML document. The selector determines which elements in the document will be styled by the CSS rules defined within that rule set. Here's a breakdown of what selectors represent.

- **Type (or Tag) Selector:** Matches elements based on their node name.

Example: p will select all <p> elements.
`p {
  color: blue;
}`

- **Class Selector:** Matches elements based on their class attribute.

Example: .highlight will select all elements with class="highlight".
`.highlight {
  background-color: yellow;
}`

- **ID Selector:** Matches a single element based on its id attribute.

Example: #header will select the element with id="header"
`#header {
  background-color: gray;
}`

- **Descendant Selector:** Matches elements that are descendants of a specified element.

Example: article p will select all <p> elements that are inside an <article> element.
`article p {
  font-size: 16px;
}`

- **Attribute Selector:** Matches elements based on their attributes and values.

Example: input[type="text"] will select all <input> elements with a type attribute value of "text".
`input[type="text"] {
  border: 1px solid black;
}`

- **Pseudo-class Selector:** Matches elements based on their state or position.

Example: a:hover will select anchor elements when they are being hovered over.
`a:hover {
  color: red;
}`

- **Grouping Selector:** Allows you to group multiple selectors together to apply the same styles.
  `h1, h2, h3 {
  font-family: Arial, sans-serif;

## 4-Which components are the CSS declarations?
A CSS declaration consists of two main components:

- **Property:** This is the aspect of the element you want to style, such as its color, font size, width, etc. It's the "what" of the declaration.

- **Value:** This specifies how you want to style the property. For example, if the property is color, the value could be red, #FF0000, rgb(255,0,0), etc. It's the "how" of the declaration.

The property and value are separated by a colon **(:)** and typically end with a semicolon **(;).**
`property: value;`

## 5-Which components are considered properties?
The components that are considered properties are:

 - **color**
- **padding**

  

### LEARN JS
## 1-What data type is a sequence of text enclosed in single quote marks?
A sequence of text enclosed in single quote marks (' ') is considered a string data type in JS.
## 2-List 4 types of JavaScript operators.

Here are four types of JavaScript operators:

- **Arithmetic Operators**: These are used to perform mathematical operations.
  - `+` (Addition)
  - `-` (Subtraction)
  - `*` (Multiplication)
  - `/` (Division)

- **Comparison Operators**: These are used to compare two values.
  - `==` (Equal to)
  - `!=` (Not equal to)
  - `>` (Greater than)
  - `<` (Less than)

- **Logical Operators**: These are used to determine the logic between variables or values.
  - `&&` (Logical AND)
  - `||` (Logical OR)
  - `!` (Logical NOT)

- **Assignment Operators**: These are used to assign values to variables.
  - `=` (Assign)
  - `+=` (Add and assign)
  - `-=` (Subtract and assign)
  - `*=` (Multiply and assign)

## 3-Describe a real world Problem you could solve with a Function.

**Problem**:
A retail store wants to calculate the total price of items after applying a discount. The store often has sales where they offer different percentage discounts on items, and they need a quick way to determine the final price after the discount.

**Solution with a JavaScript Function**:
We can create a function called `calculateDiscountedPrice` that takes in the original price of an item and the discount percentage, then returns the discounted price.

```javascript
function calculateDiscountedPrice(originalPrice, discountPercentage) {
    let discountAmount = originalPrice * (discountPercentage / 100);
    let discountedPrice = originalPrice - discountAmount;
    return discountedPrice;
}


### Making Decisions In Your Code – Conditionals.

## 1-An if statement checks a __ and if it evaluates to ___, then the code block will execute.

An if statement checks a `boolean value` and only executes a block of code if that value is `true`.

## 2-What is the use of an else if?

The `else if` statement in programming is used to introduce an additional condition to an `if` statement. It allows for multiple conditions to be checked in a sequential manner. Here's how it's used:

- The `if` statement checks its condition first.
- If the `if` condition is `false`, the program will then check the condition of the subsequent `else if` statement.
- If the `else if` condition is also `false`, the program can check another `else if` condition (if provided), and so on.
- If none of the conditions are `true`, an optional `else` block can be executed.

The primary use of `else if` is to handle multiple, distinct conditions in a clear and organized manner. It allows for more specific control flow in a program.

## 3-List 3 different types of comparison operators.

- **Equal to (`==`)**:
  - Compares two values for equality.
  - Returns `true` if the values are equal, even if they are of different data types (due to type coercion).
  - Example: `5 == "5"` would return `true`.

- **Strictly equal to (`===`)**:
  - Compares two values for equality, taking into account both value and data type.
  - Returns `true` only if the values and their data types are the same.
  - Example: `5 === "5"` would return `false`.

- **Not equal to (`!=`)**:
  - Compares two values for inequality.
  - Returns `true` if the values are not equal.
  - Example: `5 != 6` would return `true`.

There are other comparison operators as well, such as `>`, `<`, `>=`, `<=`, and `!==`, but the above three are among the most commonly used.

## 4-What is the difference between the logical operator `&&` and `||`?

The logical operators `&&` and `||` are used to combine multiple conditions in JavaScript (and many other programming languages). Here's the difference between the two:

- **Logical AND (`&&`)**:
  - Returns `true` if both operands are `true`.
  - If the first operand is `false`, it short-circuits and doesn't evaluate the second operand.
  - Example:
    ```javascript
    true && true   // Returns true
    true && false  // Returns false
    false && true  // Returns false (second operand is not evaluated)
    false && false // Returns false
    ```

- **Logical OR (`||`)**:
  - Returns `true` if at least one of the operands is `true`.
  - If the first operand is `true`, it short-circuits and doesn't evaluate the second operand.
  - Example:
    ```javascript
    true || true   // Returns true
    true || false  // Returns true
    false || true  // Returns true
    false || false // Returns false
    ```












