# 09/03/14
Using the HTML in [index.html](index.html):

- Create and link to a JavaScript file.
- Your program should execute the following steps:
  1. Get the quantities out of the input boxes and store them in variables.
  2. Use `Number("37")` to convert the strings from the input to numbers
  3. Multiply them by their cost and add them together
  4. Create a string based on that number (e.g. "37 monies")
  5. Change the total to use that string.
  6. Put all of the above steps inside a function.
  7. Assign that function to the `onclick` property of the update button.

# Functions

To make a function fire on an event, assign it to the element's event handler:

```js
document.getElementById("myBtn").onclick = function(){
  // Code goes here
};
```

# Resources
- [document.getElementById](https://developer.mozilla.org/en-US/docs/Web/API/document.getElementById)
- [element.textContent](https://developer.mozilla.org/en-US/docs/Web/API/Node.textContent)
- [input.value](http://www.w3schools.com/jsref/prop_text_value.asp)

# Level Up
- Create examples of each type and operator. Explain via comments what you think the value will be *before you run the code*. Then type it into the console to see if you were right.
- Read http://eloquentjavascript.net/03_functions.html
- Read http://eloquentjavascript.net/04_data.html
- Create 3 objects that have properties containing all of the types, with at least one function each, and one of the objects must be able to mutate both itself and another object.
- Read http://bonsaiden.github.io/JavaScript-Garden/#types.equality
