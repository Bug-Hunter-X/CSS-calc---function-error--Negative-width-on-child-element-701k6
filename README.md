# CSS calc() Function Error
This repository demonstrates a common error encountered when using the `calc()` function in CSS. The issue arises when subtracting a value from 100%, resulting in a negative width if the parent container's width is smaller than the subtracted value.

## Problem
The provided CSS code uses `calc(100% - 20px)` to set the width of a child element. If the parent's width is less than 20px, the calculation produces a negative value, causing the element to collapse or behave unexpectedly.

## Solution
The solution involves adding a `max-width` property to the child element to prevent negative widths and ensure that the element doesn't exceed the available space.  This ensures a more robust and predictable layout, regardless of the parent container's size.
