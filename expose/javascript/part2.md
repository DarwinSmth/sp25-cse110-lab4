1) 3 is printed, since the for loop uses var i, which is function scoped and not block scoped. The loop finishes when i is 3 and the loop condition becomes false. 
2) 150 is printed, since during the final iteration of the loop, discountedPrice was assigned the value 300 * 0.5, which is 150. Also because discounted is var, so it can be accessed outside of the loop even though it is declared inside.
3) 150 is printed, since final price was most recently assigned the Math.round(15000)/100.
4) The function returns [ 50, 100, 150 ], since it stores the value of the discount applied to each price during each iteration of the loop.
5) There is a ReferenceError, since i was declared within the loop and is no longer accessible after the loop.
6) Also a ReferenceError, since discountedPrice is declared within the loop block and is not accessible outside the block.
7) Since finalPrice is declared in the function scope outside of the loop, it is accessible, so it prints 150 (300 with a 0.5 discount).
8) The function returns [ 50, 100, 150 ] since each iteration of the loop stores the value of the discount applied to each price. The output is correct since all block scoped variables are referenced in their accessible blocks.
9) There is a ReferenceError, since i is still a let variable, which is not accessible outside of its block (the loop).
10) 3 is printed, since length was declared outside of the loop, so it is accessible outside of the loop.
11) The function returns [ 50, 100, 150 ] since each iteration of the loop stores the value of the discount applied to each price. All variables are declared and accessed in proper locations to avoid errors. 
12) 
  **A.** student.name  
  **B.** student['Grad Year']  
  **C.** student.greeting()  
  **D.** student['Favorite Teacher'].name  
  **E.** student.courseLoad[0]  
    
13) 
  **A.** 32, + triggers string concatenation since '3' is a string  
  **B.** 1, since - forces numeric conversion  
  **C.** 3, since null is converted to 0 in numeric context  
  **D.** 3null, + triggers string concatenation since '3' is a string  
  **E.** 4, since true is converted to 1 in numeric context  
  **F.** 0, since both false and null convert to 1 in numeric context  
  **G.** 3undefined, + triggers string concatenation since '3' is a string  
  **H.** NaN, since - forces numeric conversion and undefined -> NaN  
    
14)  
  **A.** true, since js converts string to number when comparing with a number  
  **B.** false, since both are strings and '2' comes after the '1' in '12'  
  **C.** true, since '2' is converted to a number  
  **D.** false, since === is does not allow type conversion  
  **E.** false, since true converts to 1  
  **F.** true, since Boolean returns true for any nonzero number  

15)  == is loose equality, so it compares values after converting to the same type. === compares both value and type.
16)  (part2-question16.js)
17)  When modifyArray is called, it creates a new array, and then each iteration of the loop calls the callback function (doSomething) on each value in the array that was passed in the initial modifyArray call, doubling each value, and then adding it to the new array. The result is the array [ 2, 4, 6 ].
18)  (part2-question18.js)
19)  The first line of the function prints 1 immediately, second line schedules console.log(2) to print 2 after 1 second, third line schedules console.log(3) to print after the task queue is clear, and the fourth line prints 4 immediately. so the order of numbers printed would be 1, 4, 3, 2.
