1. What is printed by line 9? If the code returns an error, explain why.
Line 9 prints "values added:  20".

2. What is printed by line 13? If the code returns an error, explain why
Line 13 prints "final result:  20".

3. What is printed by line 9? If the code returns an error, explain why. ^^^^^
Line 9 prints "values added:  20"

4. What is printed by line 13? If the code returns an error, explain why. 
The code returns an error because outside of the block governed by the if statement, result is inaccessible because the let keyword made it only visible in said block. Since we tried to use it outside of said block, a "result is not defined error" is thrown.

5. What is printed by line 9? If the code returns an error, explain why. ^^^^^

The code returns an error because we tried reassigning result when it was declared with the const keyword, meaning that we can't change its value after its initial assignment. Since we try to do just that in line 7, we get an error since this it is an illegal operation.

1. What is printed by line 13? If the code returns an error, explain why. 
Technically nothing is printed by line 13 because it seems that line never ran because the error at line 7 stopped the rest of the function from executing.