# Devtools Part 2 Questions
### Question 1
- The bug was that the values were passed in as strings by default because of .value so it ended up concatenating the two integers instead of adding them.
### Question 2
- I fixed the bug by typecasting around the two variables and using Number() to make sure it is treated as integers.