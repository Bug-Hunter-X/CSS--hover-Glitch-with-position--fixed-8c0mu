# CSS :hover Issue with `position: fixed`

This repository demonstrates an uncommon CSS bug related to the interaction between the `:hover` pseudo-class and `position: fixed`.  The `bug.css` file contains the problematic code where a fixed-positioned element's hover effect persists unexpectedly. The `bugSolution.css` file offers a solution to mitigate this unexpected behavior.  This problem arises because fixed elements are removed from the document flow, confusing the browser's hover detection.

## Problem
When hovering over an element with `position: fixed`, the hover state may remain active even after the cursor leaves the element's bounds. This can cause frustrating visual glitches.

## Solution
The solution involves using techniques such as carefully managing z-index, or using Javascript to detect mouse events and manually apply/remove the hover styles.