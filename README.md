# CSS Float Layout Bug

This repository demonstrates a common issue with floating elements in CSS that can lead to unexpected layout behavior.  The problem arises when the total width of floating elements exceeds the width of their parent container.

## Problem
The provided `bug.css` file contains CSS that uses `float: left;` on `div` elements.  If the combined width of these elements exceeds the parent's width, the parent container will collapse, and the height will be determined by the tallest floating element. Content placed after the floating elements will overlap them.

## Solution
The `solution.css` file offers a solution to fix this issue.  It adds `overflow: auto;` to the parent container. This forces the parent to accommodate the floating elements, preventing collapse and ensuring the correct layout.  Alternatively, using flexbox or grid layout can provide a more robust and flexible solution for modern layouts.