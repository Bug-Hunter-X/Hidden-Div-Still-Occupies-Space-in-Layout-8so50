# Uncommon HTML Bug: Hidden Div Still Occupies Space

This repository demonstrates a subtle bug in HTML where a div element, after having its content cleared and display set to `none`, still occupies space in the page layout.  The issue arises from the interaction of `innerHTML` and `display: none;`.

## Bug Description

The provided HTML code has a div that is initially visible.  A button, upon being clicked, clears the div's content using `innerHTML = ""`, and then hides it using `style.display = "none;"`.  Despite being hidden, the div continues to reserve space on the page, causing layout issues.

## Solution

The solution involves ensuring that the hidden element does not affect the layout.  See the `bugSolution.html` file for the corrected code.