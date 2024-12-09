# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating over arrays.  The provided `BuggyArray.java` file contains the erroneous code, and `CorrectedArray.java` shows the solution.

The bug arises from an incorrect loop condition that attempts to access an element beyond the array's bounds.

## How to Reproduce

1. Compile and run `BuggyArray.java`.  This will result in an `ArrayIndexOutOfBoundsException`.
2. Compile and run `CorrectedArray.java`.  This will run without error.

## Solution

The solution simply corrects the loop condition to `i < arr.length`, ensuring that the loop terminates before accessing an invalid index.