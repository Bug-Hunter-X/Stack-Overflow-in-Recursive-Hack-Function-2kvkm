# Stack Overflow Bug in Hack

This repository demonstrates a common error in recursive functions written in Hack: stack overflow. The `foo` function calculates the factorial of a number recursively. However, it lacks proper handling for negative inputs, leading to infinite recursion and a stack overflow.

The `bug.hack` file contains the erroneous code, while `bugSolution.hack` provides a corrected version.

## How to reproduce

1. Clone this repository.
2. Compile and run `bug.hack` with a sufficiently large positive integer or with a negative integer as input.  You will observe a stack overflow error.
3. Compile and run `bugSolution.hack`. This version handles negative inputs and prevents stack overflow.

## Solution

The solution involves adding a check to handle negative inputs, preventing infinite recursion and avoiding the stack overflow.