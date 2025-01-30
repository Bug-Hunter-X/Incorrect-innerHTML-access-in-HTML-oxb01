# Incorrect innerHTML Access in HTML
This example demonstrates an uncommon yet crucial error in HTML: Incorrectly accessing and modifying the `innerHTML` property of an HTML element without proper DOM manipulation.

## Bug Description
The primary issue is accessing `myDiv` directly using `myDiv.innerHTML` instead of using `document.getElementById('myDiv')` to get a reference to the element before modifying its content.  This approach is generally unreliable and prone to errors, particularly in larger or more complex applications.  It may work in some simplified contexts, but it's not a robust or recommended approach.

## Solution
The correct way to modify the innerHTML of an element is to first use `document.getElementById()` to get a reference to the element.  This ensures that you are working with the correct element before modifying its content.

This approach avoids potential conflicts and ensures that the modification is applied correctly.