# Part 2 Answers
1. 3 will be printed out at line 12 because the var i was iterated thorugh the loop and became added up to 3.
2. 150 will print at line 13. This is because it is what the discounted price is at the 3rd iteration of the code.
3. 150 will print at line 14 becuase this is the discounted price and it is the last iteration of it, making the discounted price of 150 the final price. 
4. This function will return a list of the discounted prices. It is a list [50,100,150]
5. At line 12, this code causes an error because i has block scope in the for loop since it is with a let declaration. At line 12, it calls `console.log(i)` which is out of scope.
6. At line 13, this code causes an error because discountedPrice has block scope within the for loop since it is with a let declaration.At line 13, it calls `console.log(discountedPrice)` which is out of scope.
7. 150 because discounted was declared outside of the for-loop. In the for loop, the finalPrice was pushed onto the list. However, since the list discounted has scope outside of the for-loop, when `console.log(finalPrice)` was called, it was defined.
8. Function will return a list of [50, 100, 150] because the discounted list was defined with let outside of the for-loop. It is still in scope and so it is still defined in and outside of the for-loop.
9. On line 11, this code causes an error because i was defined inside the scope of the for-loop. On line 11, it has a scope outside of the for-loop and i is undefined since it is out of scope.
10. 3 will print at line 12 because const first assigns length to be 3 at the beginning of the code. This value does not change and the scope reaches line 12. 
11. This function will return a list of [50, 100, 150] because while discounted is a const variable, that means it cannot be reassigned. However, it can still be mutated and elements can be added to it. Its scope on line 14 (the return) is still within the scope of where it was declared.

## Data Types
12. Objects
    1.  student.name
    2.  student['Grad Year']
    3.  student.greeting()
    4.  student['Favorite Teacher'].name
    5.  student.courseLoad[0]

13.  Arithmetic
    1.  '3' + 2 = 5. '3' is type converted to integer 3. 3 + 2 = 5
    2.  '3' - 2 = 1. '3' is type converted to integer 3. 3 - 2 = 1
    3.  3 + null = 3. Null is coverted to 0. 3 + 0 = 3.
    4.  '3' + null = '3null'. String concatenation because it is with string '3' and then null value. Null value is type converted into a string.
    5.  true + 3 = 4. True is converted to 1. 1 +3 = 4
    6.  false + null = 0. false and null is converted to 0. 0 + 0 = 0.
    7.  '3' + undefined = '3undefined'. String concatentation happens because it is with string '3' and undefined is type converted to 'undefined'
    8.  '3' - undefined = NaN. This is because '3' is converted to 3 and undefined is converted to NaN.
14.  Comparison
    1.  '2' > 1. True. '2' is type converted to 2 and 2 > 1.
    2.  '2' < '12'. False. '2' is lexicographically greater than '12'
    3.  2 == '2'. True. '2' is converted to 2. 2 == 2 which is true. 
    4.  2 === '2'. False because under strict equality check, these are of different types
    5.  true == 2. False. true is converted to 1 and 1 does not equal 2. 
    6.  true === Boolean(2). True. Boolean(2) is converted to become true. This is now of the same type and equivalence.

15. Between the == and ===, the === is a strict equality operator. In other words, === checks if items on both the left and right side are of the same type and is equivalent. It does not type convert the items on the left and right side. Therefore, when === is used, it is directly checking for true equivalence. == compares two items and type converting can be used in order to compare these elements.