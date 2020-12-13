# 9. Functions

Functions are one of the fundamental building blocks of the R language.
They are small pieces of reusable code that can be treated like any other R object.

# Syntaxys
```
 function_name <- function(arg1, arg2){
	 Manipulate arguments in some way
	 Return a value
 }
```
The "variable name" you assign will become the name of your function. arg1 and
arg2 represent the arguments of your function. You can manipulate the arguments
you specify within the function. After sourcing the function, you can use the 
function by typing:
``` 
 function_name(value1, value2)
```
If you want to see the source code for any function, just type the function name
without any arguments or parentheses.

### Function with default arguments
```
 increment <- function(number, by = 1){
     number + by
 }
```
You can also explicitly specify arguments in a function. When you explicitly
 designate argument values by name, the ordering of the arguments becomes
unimportant. You can try this out by typing: increment(by = 11, number = 5)

You can pass functions as arguments to other functions just like you can pass
data to functions.

### New Binary operators

The syntax for creating new binary operators in R is unlike anything else in
R, but it allows you to define a new syntax for your function. I would only
recommend making your own binary operator if you plan on using it often!

User-defined binary operators have the following syntax:
     %[whatever]% 
where [whatever] represents any valid variable name.
 
Let's say I wanted to define a binary operator that multiplied two numbers and
then added one to the product. An implementation of that operator is below:
```
"%mult_add_one%" <- function(left, right){ # Notice the quotation marks!
  left * right + 1
}
```
I could then use this binary operator like `4 %mult_add_one% 5` which would
evaluate to 21.

## Basics Functions

Commands:
* Returns a string representing today's date:  
  ```Sys.Date()```
* Return the average of all of the numbers in the input vector:  
  ```mean()```
* Calculate the average of all of the numbers in a vector:  
  ```mean()```
* See a function's arguments:  
```args()```  

## Swirl R Programming (Functions) Script Answers

[boring_function.R](https://github.com/bea314/datasciencecoursera/blob/main/2_R%20Programming/week%202/swirl9/boring_function.R)  
[my_mean.R](https://github.com/bea314/datasciencecoursera/blob/main/2_R%20Programming/week%202/swirl9/my_mean.R)  
[remainder.R](https://github.com/bea314/datasciencecoursera/blob/main/2_R%20Programming/week%202/swirl9/remainder.R)  
[telegram.R](https://github.com/bea314/datasciencecoursera/blob/main/2_R%20Programming/week%202/swirl9/telegram.R)  
[evaluate.R](https://github.com/bea314/datasciencecoursera/blob/main/2_R%20Programming/week%202/swirl9/evaluate.R)  
[mad_libs.R](https://github.com/bea314/datasciencecoursera/blob/main/2_R%20Programming/week%202/swirl9/mad_libs.R)  
[bin_op.R](https://github.com/bea314/datasciencecoursera/blob/main/2_R%20Programming/week%202/swirl9/bin_op.R)

Go to: [R Programming (repository)](https://github.com/bea314/datasciencecoursera/tree/main/2_R%20Programming)  
Go to: [R Programming - week1 (repository)](https://github.com/bea314/datasciencecoursera/tree/main/2_R%20Programming/week%201)

## Contributors
Date | FirstName | LastName | Email
--- | --- | --- | ---
13/12/2020 | Beatriz |  Del Pinal |  <beatrizdelpinal@gmail.com>
--/--/---- | Submit |  Pull Request | <youremailhere@gmail.com>
