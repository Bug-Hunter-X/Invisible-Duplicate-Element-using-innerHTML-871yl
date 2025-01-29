# Invisible Duplicate Element Bug in HTML

This repository demonstrates an uncommon bug related to using `innerHTML` in JavaScript to manipulate HTML elements. The bug causes a duplicated element with the same ID to become invisible.

## Bug Description
The provided HTML file uses JavaScript to replace the content of a div with new content, including another div with the same ID.  The unexpected behavior is that the newly added div is not rendered in the browser.

## Solution
The solution file demonstrates the correct approach of using DOM methods like `createElement` and `appendChild` to add elements to the DOM tree. This avoids the confusion caused by replacing content with `innerHTML`, which effectively re-interprets the entire HTML content.  It provides a cleaner and more reliable way to manage the HTML structure dynamically.

## How to Reproduce
1. Open `bug.html` in a web browser.
2. Observe that the newly created div with id 'myDiv' within the inserted paragraph is not visible.
3. Open `solution.html` to see the correct implementation.
