# Tcl String Comparison Bug

This repository demonstrates a common error in Tcl programming: using the `==` operator for string comparison instead of `eq` when comparing numbers represented as strings.  The `==` operator performs a simple string comparison, while `eq` performs a more robust comparison, considering the numerical value when comparing numbers stored as strings.

The `bug.tcl` file contains the buggy code, while `bugSolution.tcl` provides the corrected version.

## Bug Description:
The `badproc` procedure incorrectly uses `==` to compare two numbers stored as strings. This leads to wrong results because `==` compares the strings lexicographically (character-by-character), not numerically.

## Solution:
The correct way to compare numbers represented as strings in Tcl is using the `eq` operator, which handles numerical comparison correctly.
