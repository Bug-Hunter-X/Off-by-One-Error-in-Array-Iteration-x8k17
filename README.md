# Off-by-One Error in Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating through an array.  The error occurs when the loop condition incorrectly includes the last index, which is out of bounds.

## Bug Description
The provided Java code attempts to iterate through an integer array, assigning values to each element. However, due to an off-by-one error in the for loop's condition, it attempts to access an index that is beyond the array's bounds, leading to an `ArrayIndexOutOfBoundsException`.

## Bug Solution
The solution corrects the loop condition to ensure it iterates only up to `arr.length - 1`, avoiding the out-of-bounds access.

## How to reproduce
1. Clone this repository.
2. Compile and run the `Bug.java` file.  This will result in the exception being thrown.
3. Replace `Bug.java` with `BugSolution.java` and compile and run again to observe the corrected behavior.