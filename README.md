# JavaScript Function: Unexpected NaN Handling in Addition

This repository demonstrates a subtle bug in a JavaScript function related to handling NaN (Not a Number) values during addition. The original function (`bug.js`) doesn't explicitly handle NaN, leading to unexpected results.  The corrected version (`bugSolution.js`) addresses this issue by incorporating specific NaN checks.

## Bug Description

The `foo` function attempts to add two numbers, but it fails to handle the case where one or both inputs are NaN.  This can lead to unexpected behavior in applications that rely on this function's output to perform further calculations.

## Solution

The corrected function (`bugSolution.js`) adds a check for NaN using `isNaN()`. If either input is NaN, the function returns a predefined value (0, in this case) to prevent propagation of NaN. This provides more robust error handling and predictable behavior.