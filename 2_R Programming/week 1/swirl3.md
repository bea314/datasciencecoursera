# 3. Sequences of Numbers

* Questions about a particular R function:  
```?function_name_here```  
Note: In the case of an operator like the colon used above, you must enclose the symbol in backticks like this: ``` ?`:` ```.

## Creating sequences of numbers

* Create a sequence of numbers in R by using:  
  ``` `:` ```  
  ```seq()```  
  e.g.  
  seq(0, 10, by=0.5), seq(5, 10, length=30)
  
* Length of a vector:  
  ```length()```
  
* Vector of same length:  
  ```seq(along.with = my_seq)```  
  ```1:length(my_seq)```  
  ```seq_along(my_seq)```
  
* Replicate a number in x length:  
  ```rep()```  
  e.g.  
  rep(0, times = 40)  
  rep(c(0, 1, 2), each = 10)
  
Go to: [R Programming (repository)](https://github.com/bea314/datasciencecoursera/tree/main/2_R%20Programming)  
Go to: [R Programming - week1 (repository)](https://github.com/bea314/datasciencecoursera/tree/main/2_R%20Programming/week%201)

## Contributors
Date | FirstName | LastName | Email
--- | --- | --- | ---
12/12/2020 | Beatriz |  Del Pinal |  <beatrizdelpinal@gmail.com>
--/--/---- | Submit |  Pull Request | <youremailhere@gmail.com>
