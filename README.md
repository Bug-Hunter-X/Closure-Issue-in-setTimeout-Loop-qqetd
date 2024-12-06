# JavaScript Closure Issue in setTimeout Loop

This example demonstrates a common issue with closures in JavaScript's `setTimeout` function when used within a loop.  The expected behavior is to print numbers 0-9 with a one-second delay. However, due to how closures work, the value of `i` is captured only after the loop finishes, resulting in the unexpected output of 10 ten times.

The `bug.js` file contains the buggy code, while `bugSolution.js` provides a solution using an immediately invoked function expression (IIFE) to capture the correct value of `i` for each iteration.