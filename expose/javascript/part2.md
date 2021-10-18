1. `3` will be printed. Since the for loop uses `var i`, the variable declaration will be hoisted to
the top level function scope. This makes the variable visible on line 12 (and also means it retains its final value
after the for loop terminates.

2. `150` will be printed. Since `discountedPrice` is defined via `var`, the declaration will be hoisted to the top level
function scope. Thus, when the loop terminates, discountedPrice will be the discount applied to the last element in the
array; and, since the declaration was hoisted, the variable is in scope even outside of the for loop.

3. `150` will be printed. Since `finalPrice` is declared at the top function level, and variables defined with var are
visible at function scope, the final price variable will be in scope at line 14. Additionally, it will take the value of
`Math.round(discountedPrice * 100) / 100 which is `150` on the last iteration of the loop. Thus, it prints 150.

4. This function will return this array: `[50, 100, 150]`. This is because the for-loop computes the 50% of each array
value and pushes that value into a new array. This new array is then returned.

5. error - Since the variable i is defined using a let statement, it is not visible outside the for-loop. Thus, line 12
creates a reference error.

6. error - Since the variable discountedPrice was defined using a let statement, it's scope is restricted to the
for-loop block. Thus, it is not visible outside of the for-loop, meaning line 13 causes a reference error.

7. `150` will be printed. Since `finalPrice` is declared at the top function level with a let statement, it will have
block scope, which here is the function's scope. Thus, it will be visible on line 14. And since the for-loop's last
iteration computes `300 * 0.5`, line 14 will print `150`.

8. Returns an array of the followign form: `[50, 100, 150]`. Since the function's for-loop computes half the value of each element
in the array and pushes it to a new array, the new array ends up with the values listed prior.  

9. error - Since the variable i is defined using a let statement, it is not visible outside the for-loop. Thus, line 11
creates a reference error. 

10. `3` will be printed. Since the array passed in has a length 3, and length is only assigned once, the variable
length's value will be 3 when at line 12.

11. Returns an array of size 3 with these elements: [50, 100, 150]. Since only the array reference is const, it's
permissible to modify the contents of the array. Thus, the array becomes populated with 50% of the value of each element
in prices.

12A. `student.name`
12B. `student['Grad Year']`
12C. `student.greeting()`
12D. `student['Favorite Teacher'].name`
12E. `student.courseLoad[0]`

13. A. outputs `'32'` - `2` is converted to a string and then both strings are concatenated.

13. B. outputs `1` - `3` is converted to a number type and then numeric subtraction occurs.

13. C. outputs `3` - null is converted to an int and its value as an int is 0.

13. D. outputs `'3null'` - null is converted to a string with value 'null' and then concatenation occurs.

13. E. outputs `4` - true is converted to a number with value 1 and then numeric addition occurs.

13. F. outputs `0` - false is converted to a number with value 0 and null is converted to a number with value 0 and then
numeric addition occurs.

13. G. outputs `'3undefined'` - undefined is converted a string with value 'undefined' and then string concatenation
occurs

13. H. outputs `NaN` - '3' is converted to an int with value 3 and undefined is converted to a number with value NaN.
Then, numeric subtraction occurs, but subtracting NaN results in NaN.

14. A. outputs `true` - '2' is converted to a number and then the greater than comparison is made, which outputs true
since 2 > 1.

14. B. outputs `false` - string vs string comparison here is done by lexicographical ordering. Since '1' comes before '2' in lexicographic ordering, the second argument is less than the first.

14. C. outputs `true` - string '2' is converted to numeric 2 and then the equality becomes 2 == 2, which is true.
  
14. D. outputs `false` - no type conversion is performed, so since the types are mismatched, this outputs false.
  
14. E. outputs `false` - true is converted to a number with value 1 and then the equality check is performed as 1 == 2 which is false.
  
14. F. outputs `true` - Boolean(2) converts 2 to a boolean, with value true. Then the comparison becomes true === true, which is true.

15. `==` allows for type conversion (i.e. `'2' == 2` is true) whereas `===` does not permit type conversion, so each
operand must be equal in both type and value.

16. js file

17. outputs an array of the following form: `[2, 4, 6]`. Each iteration of the for loop extracts a value from the
original array, executes the callback, and pushes that return value into the new array. Since the callback function just returns its argument
multiplied by 2, this means each iteration of the array essentially takes the original array's value and doubles it.
This is why the new array has the same size but contains values 2x greater than the original array.

18. js file

19. outputs 1, 4, 3, 2 (note each is outputted on its own line with no commas).
