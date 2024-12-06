# Silent Error in Division Function

This repository demonstrates a common, yet subtle error in JavaScript: silent failure due to division by zero. The `foo` function is designed to divide `a` by `b`, however, it doesn't correctly handle the cases where either `a` or `b` is zero.

## The Bug

The `bug.js` file contains the erroneous code.  When either `a` or `b` is 0, the function will throw an error, which is unexpected behavior and could cause your application to crash. Also, when both a and b are 0, it will throw an error. The expected behavior is that it should return 0 for this case.  This illustrates a situation where silent error handling can lead to unexpected application behavior.

## The Solution

The solution is provided in `bugSolution.js`.  A robust error handling mechanism has been implemented using a simple check to prevent division by zero and explicit return 0 when either a or b is 0 and return 0 when both are 0.