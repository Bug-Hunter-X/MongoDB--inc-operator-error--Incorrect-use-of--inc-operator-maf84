# MongoDB $inc operator error: Incorrect use of $inc operator
This example demonstrates an error caused by using a string value with the `$inc` operator in a MongoDB update query. The correct usage is to supply a numerical value to the `$inc` operator to increment the field by the given value.  Using a string results in no increment.

## Bug
The `bug.js` file contains code that attempts to increment a counter field in a MongoDB document using the `$inc` operator, but passes a string as the increment value.  This leads to the field not being incremented.

## Solution
The `bugSolution.js` file shows the corrected code, which uses a numeric value for the increment, successfully updating the field.  This ensures the field is correctly incremented.