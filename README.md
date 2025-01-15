# JavaScript TypeError: Cannot read properties of undefined (reading 'length')

This repository demonstrates a common JavaScript error: `TypeError: Cannot read properties of undefined (reading 'length')`.  This error occurs when attempting to access the `length` property of a variable that is `undefined`.

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides a corrected version.

## Bug
The bug arises from not handling the case where the input to the function `foo` is `undefined`.  Accessing `.length` on `undefined` results in the error.

## Solution
The solution involves explicitly checking if the input is `undefined` before attempting to access its `length` property.  A simple check using `typeof x === 'undefined'` or a nullish coalescing operator (`x ?? []`) effectively prevents the error.