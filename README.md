# MongoDB $inc operator with String value error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries. The error arises from providing a string value instead of a numeric value to the `$inc` operator, resulting in an incorrect update.

## Bug Description
The bug is caused by using a string '1' instead of a number 1 with the $inc operator. This leads to the operator treating the string as a field name instead of a value to increment. This results in adding a new field instead of incrementing the count field. 

## Solution
The solution is to use a numeric value (integer or floating point number) with the `$inc` operator to correctly increment the count field.  This ensures that the `$inc` operator functions as intended, adding the numeric value to the existing field value.