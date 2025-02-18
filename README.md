# Javascript Loose vs Strict Equality with Null and Undefined

This repository demonstrates a common yet subtle error in JavaScript involving the comparison of null and undefined values using loose (==) versus strict (===) equality.

## The Problem

The loose equality operator (==) performs type coercion before comparison, leading to unexpected results when comparing null and undefined.  Strict equality (===), on the other hand, does not perform type coercion and provides more predictable behavior.

## Code Example

The `bug.js` file contains code illustrating this issue, showcasing how loose equality can inadvertently handle undefined values as equivalent to null which can be problematic when relying on explicit null checks.

## Solution

The `bugSolution.js` file demonstrates the recommended approach of using strict equality (===) for precise comparison of null and undefined, avoiding ambiguity and potential errors.