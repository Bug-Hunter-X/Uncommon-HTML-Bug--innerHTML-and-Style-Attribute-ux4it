# Uncommon HTML Bug: innerHTML and Style Attribute

This repository demonstrates an uncommon bug related to using `innerHTML` to modify the `style` attribute of an HTML element.  The issue arises from how the browser handles style updates within the `innerHTML` string.  While seemingly simple, this behavior can be confusing and lead to unexpected display issues.

## Bug Description
The provided HTML file attempts to set the display style of a div to 'none' using `innerHTML`.  The solution shows how to correctly modify the style attribute using the `style` property of the DOM element.

## How to reproduce
1. Clone the repository.
2. Open `bug.html` in your web browser.
3. Observe that the text within the div is still visible, even though the `innerHTML` modification attempts to set `display: none;`.

## Solution
The `bugSolution.html` file provides the corrected code that correctly hides the element.

This example highlights the importance of understanding how the browser handles DOM updates and manipulations, especially when involving styling through string concatenation within `innerHTML`.