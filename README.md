# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates an uncommon bug related to the use of `innerHTML` in HTML.  While seemingly simple, repeatedly using `innerHTML +=` to append multiple elements can lead to unexpected behavior and reduced performance. This example shows the problem and provides a corrected approach using `createElement`.

## Bug Description
The original code directly adds multiple HTML elements using `innerHTML +=`. This is generally less efficient and can cause problems if the added HTML contains already existing ids or other elements that may conflict with the current DOM structure.

## Solution
The solution demonstrates the preferred method of creating elements with `document.createElement`, setting content with `document.createTextNode`, and then appending them to the parent element using `appendChild`. This method improves efficiency and maintains clarity in DOM manipulation.

## How to run
1. Clone the repository
2. Open `bug.html` in your web browser to see the buggy implementation.
3. Open `bugSolution.html` to see the corrected implementation.