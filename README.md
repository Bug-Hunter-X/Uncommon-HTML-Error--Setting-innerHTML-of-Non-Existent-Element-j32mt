# Uncommon HTML Error: innerHTML on Non-Existent Element

This repository demonstrates a subtle error in HTML that can be difficult to catch. The error occurs when attempting to set the `innerHTML` property of an element that does not exist in the DOM.

## The Bug

The `bug.html` file contains JavaScript code that attempts to set the `innerHTML` of an element with the ID 'nonExistentElement'.  Since this element is not present in the HTML, a JavaScript error is thrown.

## The Solution

The `bugSolution.html` file demonstrates the solution:  Always check if the element exists before attempting to modify it using `getElementById`.  Using `getElementById` will return `null` if the element doesn't exist, preventing the error.