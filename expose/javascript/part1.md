1) Since add is true, the if statement runs, resulting in the var result to have the value 20, printing "values added: 20"
2) Since var result can be accessed outside of the its block, "final result: 20" will be printed.
3) Having a variable be accessible outside of its block can lead to unexpected behavior. Var declaration are also hoisted to the top of the function, which can cause unexpected behavior is it is assumed to be undefined. Unlike const and let, var doesn't throw an error if accessed before declaration, instead returning undefined, which can cause unexpected bugs.
4) "values added: 20" will be printed, since the if statement is triggered due to add being true.
5) A ReferenceError is triggered because let has block scope, so it is no longer accessible outside of the block, where the log is.
6) Nothing is printed since the code returns an TypeError before the log at "result = num1 + num2;", since const requires the variable to be assigned only once, and this line attempts to reassign it.
7) Nothing is printed for the same reason given in Q6