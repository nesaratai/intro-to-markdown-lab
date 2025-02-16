#Writing a Function in JavaScript

In *JavaScript,* functions are blocks of reusable code. They allow you to bundle functionality, make it more readable, and avoid repetition. Here's a brief tutorial on writing an arrow function in JavaScript.

**1. Basic syntax**
```javascript
const functionName = (params) => {
  // code to be executed
}
```
**const:** const should be used whenever a function expression is assigned to a variable.
**The function name:** The name you choose for the function.
**Parameters:** Optional comma separated parameters. This is the data passed into the function. If there are no parameters, the () is still required.
**The arrow syntax:** Indicates that this will be a function.
**The body:** The statements that make up the function itself. Surrounded by curly braces.

Example:
```javascript
const greet = (name) => {
  console.log("Hello, " + name + "!");
}
```
***Tip:*** Functions often perform actions, so naming with a verb can make it clear what the function does. Examples include fetchData( ), calculateArea( ), or printReport( ). 

**2. Calling a function**

To execute the function, you call or invoke it by using its name followed by parentheses.

Example:

`greet('Alice');` // Outputs: Hello, Alice!

**3. Return values**

Functions can process data input and output a value using the return keyword.

Example: 
```javascript
const addNums = (numA, numB) => {
  return numA + numB
}
```
```javascript
const total = addNums(2, 4);
```

`console.log(total)` // Expected value: 6

*For more information on functions and how they are used in JS, check out the MDN docs.*
*[Mozilla]https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions*



**#DOM Events in JavaScript**

DOM (Document Object Model) events allow us to interact with HTML elements dynamically. Events like click, mouseover, keydown, and input help make web pages interactive.

Here’s a simple example where clicking on a paragraph changes its text and color:
```javascript
  // Select the paragraph and button
  let paragraph = document.getElementById("myParagraph");
  let resetButton = document.getElementById("reset");

  // Add a click event listener to change text and color
  paragraph.addEventListener("click", function () {
    paragraph.textContent = "You clicked me!";
    paragraph.style.color = "red";
  });

  // Reset the paragraph text and color when clicking the button
  resetButton.addEventListener("click", function () {
    paragraph.textContent = "Click me to change!";
    paragraph.style.color = "black";
  });
```
##Explanation
1. addEventListener("click", function ({ ... })) → Attaches a click event to the <p>.
2. textContent → Changes the paragraph text.
3.	style.color → Modifies the paragraph color.
4.	Reset Button → Restores the original text and color when clicked.

##Other Common Events

**Event Type Description**
***mouseover*** When the mouse hovers over an element
***keydown*** When a key is pressed on the keyboard
***input*** When text is typed into an input field
***dblclick*** When an element is double-clicked