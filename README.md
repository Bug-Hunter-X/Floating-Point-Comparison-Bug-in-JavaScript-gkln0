# Floating-Point Comparison Bug
This repository demonstrates a common error in JavaScript related to comparing floating-point numbers for equality.  Due to the inherent limitations of floating-point representation, direct equality checks often produce unexpected results. The bug.js file contains the erroneous code, while bugSolution.js offers a corrected approach.

## Problem
The `foo` function in `bug.js` intends to check if two numbers are equal. However, when dealing with floating-point numbers, the comparison using the strict equality operator (`===`) can fail due to rounding errors in the underlying representation.  This can lead to unexpected behavior in applications involving calculations or comparisons of floating-point values. 

## Solution
The `bugSolution.js` file demonstrates the preferred method of comparing floating-point numbers for near-equality.  This approach considers a tolerance range to account for potential rounding discrepancies and avoids the issues caused by direct equality checks. 