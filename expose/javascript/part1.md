# Part 1 Questions
### Question 1
- Line 9 prints ```values added: 20```.
### Question 2
- Line 13 prints ```final result: 20``` since the result variable is declared using var, which allows it to be accessed in the function.
### Question 3
- You should not use ```var``` because you want to avoid accidentally referencing a variable that should've been restricted to a specific loop or if statement, causing some bug later on. Moreover, it allows redeclaration of variables which could lead to accidentally overwriting preexisting data.
### Question 4
- Line 9 prints ```values added: 20```.
### Question 5
- Because ```result``` was declared with a let, it restricts the scope to just that if statement. There will be an error by line 13 because it tries to use the variable which is unaccessible since line 13 is outside of the if statement.
### Question 6
- Because ```result``` was declared with a const, line 7 will cause a TypeError because it tries to change a constant variable. Thus, it will not reach line 9 and will not print anything.
### Question 7
- Similar to question 6, because ```result``` was declared with a const, line 7 will cause a TypeError because it tries to change a constant variable. Thus, it will not reach line 13 and will not print anything.