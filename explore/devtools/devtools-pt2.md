What was the bug?

The issue is that num1 and num2 are strings. So when they are "added" in calculateSum, they are just being concatenated instead. If we sent a breakpoint at line 12 we can see this is the case as result has type string after it is initialized to num1 + num2 when it should be a number.

How would you fix it? 
We can just typecase num1 and num2 to be a number using the Number() function.