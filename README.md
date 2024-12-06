# Unexpected String Concatenation in JavaScript Function

This repository demonstrates a common yet subtle bug in JavaScript: unexpected string concatenation when adding a number and a string.  The `foo` function intends to perform numerical addition, but due to JavaScript's type coercion, it performs string concatenation instead.

## Bug Description

The function `foo` takes two arguments, `a` and `b`. When one argument is a number and the other is a string, the `+` operator performs string concatenation, rather than numerical addition. This results in an unexpected output.

## Solution

The solution involves explicitly converting the arguments to numbers before performing the addition. The `Number()` function is used to achieve this. 

## How to reproduce the bug
1. Clone this repository.
2. Open `bug.js` in a code editor or JavaScript environment.
3. Run the code using `node bug.js` or a similar command.