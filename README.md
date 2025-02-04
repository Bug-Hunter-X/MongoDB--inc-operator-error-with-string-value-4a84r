# MongoDB $inc operator error with string value
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numeric field by a specified value.  However, if a string is provided as the increment value, MongoDB will throw an error.

## Bug Description
The bug lies in the incorrect usage of the `$inc` operator. The value being incremented should be a number, not a string.  Attempting to increment with a string results in an error.

## Solution
The solution involves ensuring that the value provided to the `$inc` operator is a number.  This is shown in the `bugSolution.js` file.
