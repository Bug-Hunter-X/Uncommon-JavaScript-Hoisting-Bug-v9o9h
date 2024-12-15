# Uncommon JavaScript Hoisting Bug

This repository demonstrates a subtle bug related to JavaScript's hoisting mechanism. The code in `bug.js` showcases an unexpected behavior due to the interaction between variable declarations and their usage within a function's scope.

## Bug Description

The script uses the variable 'a' before it's declared. It might be expected to result in a ReferenceError, but due to hoisting, it logs 'undefined' instead.  This behavior might be unexpected for developers unfamiliar with the subtleties of hoisting in JavaScript.

## Solution

The `bugSolution.js` file demonstrates the corrected code. By moving the `console.log` statement after the variable declaration, the correct value of 'a' (1) is logged to the console.