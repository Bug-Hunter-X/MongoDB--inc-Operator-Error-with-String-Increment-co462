# MongoDB $inc Operator Error
This example demonstrates an error that occurs when using the `$inc` operator in MongoDB's `updateOne` method with an incorrect data type.  The `$inc` operator is designed to increment a numerical value, and attempting to increment with a string will result in an error.

## Bug
The bug is caused by passing a string value ('1') to the `$inc` operator, which expects a number.  This leads to a MongoDB operation error.

## Solution
The solution is to change the increment value to a number (1).