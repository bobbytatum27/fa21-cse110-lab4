1. The statement `document.getElementById("num1").value;` returns a string. Thus, when the input numbers (First Number,
Second Number) are passed as arguments to the
function calculateSum, the `result` variable becomes the result of a concatenation operation on two strings. If the
strings were instead number types, then the addition operation would add the two numbers as expected.

2. I would fix the bug by casting the input arguments to a float. This can be done with the `parseFloat` function. I
chose this function since it can convert strings that contains characters even after the numeric input (ex: 3.14fjdsja),
whereas Number() cannot. 
