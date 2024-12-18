# Unexpected Null Handling in JavaScript Addition Function

This repository demonstrates a subtle bug related to null handling in a simple JavaScript addition function.  The function is designed to add two numbers, but it unexpectedly returns `null` if either input is `null`, regardless of whether the other input is a valid number. This behavior might lead to unexpected results and errors in applications where null values might occur.

The `bug.js` file contains the function with the flawed null handling. The `bugSolution.js` file provides a corrected version of the function that addresses the issue. The solution demonstrates how to explicitly check for `null` values and treat them as 0 for more predictable and robust behavior.

## How to Reproduce
1. Clone the repository.
2. Open `bug.js` and observe the unexpected `null` return values.
3. Compare it with the improved null handling in `bugSolution.js`.

## Solution
The solution handles `null` values gracefully by explicitly checking for null and treating them as zero before performing the addition. This eliminates the unexpected `null` returns, ensuring that the function behaves predictably in various scenarios.