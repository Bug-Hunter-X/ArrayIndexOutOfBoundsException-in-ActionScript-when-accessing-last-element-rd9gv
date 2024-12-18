# ActionScript ArrayIndexOutOfBoundsException Bug
This repository demonstrates a common error in ActionScript when attempting to access the last element of an array using the length property.  ActionScript arrays are zero-indexed, meaning the first element is at index 0.  Therefore, the last element is at index myArray.length - 1.  Accessing myArray[myArray.length] will always result in an ArrayIndexOutOfBoundsException.

This example provides both the erroneous code and the corrected version.

## Bug
The bug lies in accessing the last element of an array using `myArray[myArray.length]`.  ActionScript arrays are zero-indexed, so the last element is at `myArray.length - 1`.

## Solution
The solution is to access the last element using `myArray[myArray.length - 1]`. This simple adjustment will prevent the exception.
