# Part 2 Questions
### Question 1
- This line prints the value of i at that point. `prices.length` is equal to 3 because there are 3 elements in the array. The for loop sets i equal to 0 then keeps running until i !< 3, that's when i == 3. 
- Thus, line 12 outputs the value of i which is `3`.
### Question 2
- The for loop goes through and calculates the discount for each price using the variable `discountedPrice`. Since the variable was declared with var, line 13 is able to access it and since the for loop ends at the last element, `discountedPrice`'s last value is 300 * 0.5, which is 150. 
- Thus, line 13 outputs this value of `150`.
### Question 3
- `finalPrice` in the for loop calculates the rounded version of the discounted price. As explained in question 3, the for loop runs until the last element and since the last element is `150` (which is a whole number), rounding does not change anything and thus the last value stored in `finalPrice` is `150`. This is accessible outside of the for loop because it was declared with var. 
- Thus, line 14 outputs this value of `150`.
### Question 4
- This function returns an array of the discounted prices from `prices` by applying the `discount` for each of them.
- Thus, it would return `[50, 100, 150]`.
### Question 5
- Since we declared the variable `i` with let, line 12 will cause an error as it tries to access a let variable (which is scoped only in the for loop).
### Question 6
- Similarly to question 6, the `discountedPrice` is declared with let, so line 13 trying to access it will cause an error as the scope is only in the for loop.
### Question 7
- Since `finalPrice` was declared at the function level at line 4, line 14 is still able to access the value. In the for loop, the last value stored to `finalPrice` is `150` because it is the last element in the prices array after rounding the discounted version. 
- Thus, line 14 outputs `150`.
### Question 8
- Since the `discounted` variable was declared at the function level, line 16 is still able to access the variable. This function returns an array of the discounted prices from `prices` by applying the `discount` for each of them.
- Thus, it would return `[50, 100, 150]`.
### Question 9
- Because the variable `i` was declared with a let in the for loop, line 11 will cause an error as it tries to access the value of `i`, which is only scoped in the for loop. 
### Question 10
- The variable `length` is obtained by taking the length of the array prices, which is 3 because it has 3 elements. 
- Thus, line 12 outputs `3`.
### Question 11
- Although `discounted` is declared with a const which means it is not allowed to be redeclared, modifying the contents is okay. The for loop  returns an array of the discounted prices from `prices` by applying the `discount` for each of them.
- Thus, the function returns `[50, 100, 150]`.
### Question 12
- A. `student.name`
- B. `student['Grad Year']`
- C. `student.greeting()`
- D. `student['Favorite Teacher'].name`
- E. `student.courseLoad[0]`
### Question 13
- A. '3' + 2 = `32` because of the '' around the 3, it causes it to be treated as a string and the + for strings concatenates rather than add.
- B. '3' - 2 = `1` because although 3 is a string, but the - causes it to be treated as an integer and subtracts as normal.
- C. 3 + null = `3` because null gets converted to 0 when doing arithmetic operations on them, causing it to be 3 + 0.
- D. '3' + null = `3null` because the 3 is treated as a string and the + concatenates them, so null is treated as a string too.
- E. true + 3 = `4` because true is converted to become 1 when doing arithmetic operations on them.
- F. false + null = `0` because both false anad null are converted to 0, so we get 0 + 0, which is just 0.
- G. '3' + undefined = `3undefined` because 3 is a string and + concatenates them, treating undefined as a string too.
- H. '3' - undefined = `NaN` because of the -, 3 is treated as a number and undefined is converted to NaN, so we get 3 - NaN = NaN.
### Question 14
- A. '2' > 1 = `true` because '2' is converted to an integer since 1 is also an integer, and since 2 > 1, the result is true.
- B. '2' < '12' = `false` because both are strings, so it is compared lexicographically, since 1 is before 2, the result is false.
- C. 2 == '2' = `true` because '2' is converted to an integer and since 2 is equal to 2, the result is true. 
- D. 2 === '2' = `false` because doing === compares both the values and the type, since they are not the same type, the result is false.
- E. true == 2 = `false` because the true is converted into 1 and since 1 is not equal to 2, the result is false.
- F. true === Boolean(2) = `true` because Boolean(2) checks that 2 is a non-zero number and since that is true, it is true === true, so the result is true.
### Question 15
- The key difference is that `==` compares the values after type conversion (loose equality) so it allows for type coercion whereas `===` compares the values before type conversion (strict equality) as in both the type and value must match.
### Question 16
- Answer written in `part2-question16.js`
### Question 17
- The function is called with array `[1, 2, 3]` and the function `doSomething` is passed as the `callback` argument.
- In the for loop, it iterates throuhg each element of the input array:
  - `(i = 0)` Takes in the 1st element of 1 and passes it into doSomething, doSomething(1) does 1 x 2 = 2. This is pushed into `newArr`.
  - `(i = 1)` Takes in the 2nd element of 2 and passes it into doSomething, doSomething(2) does 2 x 2 = 4. This is pushed into `newArr`.
  - `(i = 2)` Takes in the 3rd element of 3 and passes it into doSomething, doSomething(3) does 3 x 2 = 6. This is pushed into `newArr`.
- The loop ends and the function returns newArr which is `[2, 4, 6]`
- `modifyArray` essentially applies whatever callback does onto the input array and returns that resulting array.
### Question 18
- Answer written in `part2-question18.js`
### Question 19
- The output is:
```
1
4
3
2
```
- This is because the setTimeout functions are sent to a task queue and can only run once the main script is done, reuslting in the 0ms delay printing before the 1s delay.