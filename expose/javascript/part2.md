1. What will happen at line 12 and why? If the code causes an error, explain why. 

At line 12, "3" is printed to the console because the value of i after the for loop is 3 since the length of the prices array is 3 during the function call. It is important to note that because i was declared with var, it is accessible to anything inside the function (discountPrices), which is why it was able to be referenced outside of the for loop.

2. What will happen at line 13 and why? If the code causes an error, explain why. 
   
At line 13, "150" is printed because disocuntedPrice is set to 300*0.5=150 in the final iteration of the for loop. Since discountedPrice also has function scope due to the var keyword, it is accessible outside of the for loop to anything inside the discountPrices function and not just inside the loop.

3. What will happen at line 14 and why? If the code causes an error, explain why. 

At line 14, "150" is printed because it is set to 150*100/100 = 150 during the final iteration of the for loop. Since finalPrice was initialized with the var keyword at line 4, it is accessible everywhere inside the function discountPrices.

4. What will this function return? Give a brief explanation why. If the code causes an error, explain why
   
This function will return an array of ints where the prices have been reduced by half relative to the input ([50, 100, 150]). This is because the code essentially loops through each element in the input array, discounts it by discount*100 percent, and stores that discounted price into a new array which is returned at the end of the function. All of the variables have function scope so they are all visible when they are referenced.

5. What will happen at line 12 and why?  If the code causes an error, explain why

This code causes an error because i was initialized with the let keyword, which only allows it to be accessible within the block it is initialized in. Since it was initialized in the for loop, it can only be used in the body of the for loop. Thus, when we try to access it outside of it, we get a reference error.

6. What will happen at line 13 and why? If the code causes an error, explain why.

This code causes an error because discountedPrice was initialized with the let keyword, which only allows it to be accessible within the block it is initialized in. Since it was initialized in the for loop, it can only be used in the body of the for loop. Thus, when we try to access it outside of it, we get a reference error

7. What will happen at line 14 and why? If the code causes an error, explain why.

At line 14, "150" is printed because it is set to 150*100/100 = 150 during the final iteration of the for loop. Since finalPrice was initialized with the let keyword at line 4, it is accessible everywhere inside the block it was defined in, which happens to be the function discountPrices.

8. What will this function return? Give a brief explanation. If the code causes an error, explain why.

This function will return an array of ints where the prices have been reduced by half relative to the input ([50, 100, 150]). This is because the code essentially loops through each element in the input array, discounts it by discount*100 percent, and pushes that discounted price into a new array which is returned at the end of the function. All of the variables are visible in the block they are referenced so there are no errors. 

1. What will happen at line 11 and why? If the code causes an error, explain why.

This code causes an error because we are trying to reference i outside of the scope it is visible in. Since it was initialized inside the for loop with the let keyword, i is only reference-able inside of the for loop.

10.  What will happen at line 12 and why? If the code causes an error, explain why

At line 12, "3" is printed because it is the value length is set to at line 4 of the function and since length is never reassigned, there is no error. Since it was defined with the cost keyword in the function block it is also accessible when referenced in console.log. It is interesting to note however that pushing values into the const array discounted appears to not throw an error. This is because while const makes it so that the variable cannot be reassigned, it doesn't give any restrictions to whether or not the value of that variable can be changed. Since we never reassign discounted to something else and only modify its array, we avoid any errors.

11. What will this function return? Give a brief explanation. If the code causes an error, explain why.

This function will return an array of ints where the prices have been reduced by half relative to the input ([50, 100, 150]). This is because the code essentially loops through each element in the input array, discounts it by discount*100 percent, and pushes that discounted price into a new array which is returned at the end of the function. All of the variables are visible in the block they are referenced in and there is no reassigning of const variables so no errors are thrown.

12. 
Accessing the value of the name property in the student object
student.name
Accessing the value of the Grad Year property in the student object
student["Grad Year"]
Calling the function for the greeting property in the student object
student.greeting()
Accessing the name property of the object in the Favorite Teacher property in student
student["Favorite Teacher"].name
Access index zero in the array of the courseLoad property of the student object
student.courseLoad[0]

13. Arithmetic
‘3’ + 2
'32' because the int 2 maps to the string '2'

‘3’ - 2
1 because the string '3' maps to the int 3

3 + null
3 because null gets converted into 0 when added to an int

‘3’ + null
'3null' because null becomes 'null' when concatenated with a string

true + 3
4 because true gets converted into 1 when added to an int

false + null
0 because false first gets converted into 0 which causes null to be converted into 0 as well. 0. 0+0 = 0

'3' + undefined
'3undefined' because undefined gets converted into 'undefined'

'3' - undefined
NaN, '3' gets converted into the int 3, which causes undefined to be converted to NaN. 3 - NaN = NaN

14. Comparison
‘2’ > 1
true since Javascript converts values of different types into numbers. 2 > 1 is true. 

‘2’ < ‘12’
false since these are both strings so they are compared lexicographically letter by letter. '2' > '1' so this is false.

2 == ‘2’
true since Javascript converts values of different types into numbers. 2 == 2 is true. 

2 === ‘2’
false, === is a string equality check, since they are different types they are different

true == 2
false since Javascript converts values of different types into numbers. 1 == 2 is false.

true === Boolean(2)
true since boolean(2) turns 2 into true. true and true are the same type and are the same value so this is true.

15. Explain the difference between the == and === operators.
== converts the values into the same type before making a comparison whereas === compares the values without any type conversion. This means that if two values are of different types, they cannot be equal.

16. Given the above Object, write a for...in loop that will iterate through it and print out the value of the property if the property starts with the letter r, or if the value of that property is an odd number. 

See part2-question16.js

17. If the function above is called with the following parameters modifyArray([1,2,3], doSomething), what will be the result? Briefly walk through how you arrived at that result. 

The resulting output will be an array with the values [2,4,6]. in modifyArray, the for loop will iterate over all of the elements in the input array. For each element, it will push the output of calling callback (which is just the function doSomething) with the argument being said element. In doSomething, the element that is passed in as input is doubled and returned to the caller. Thus, for each element in the input array, we end up pushing 2 times that value into a new array and return that array.

18. The above program only prints out the time once when executed. Modify this code such that the program prints out the time every second.

See part2-question18.js

19. What is the output of the above code? 
```
1
4
3
2
```