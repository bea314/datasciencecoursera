# 8. Logical

There are two logical values in R, also called boolean values. They are TRUE and FALSE.
In R you can construct logical expressions which will evaluate to either TRUE or FALSE.

### TRUE / FALSE

Commands:
* If the argument evaluates to TRUE, the function will return TRUE. Otherwise, the function will return FALSE:  
  ```isTRUE()```
* Return TRUE if the two R objects passed to it as arguments are identical:  
  ```identical()```
* Exclusive OR:  
  ```xor()```
* Function to find indices:  
```which(ints > 7)```  
```any(ints < 0)```  
```all(ints > 0)```
* Function to create a random vector:  
  ```sample(10)```

Operator | Symbol
--- | ---  
equal | == 
not equal / not | !=
less than | <
grater than | >
less-than-or-equal-to | <=
greater-than-or-equal-to | >=
AND | & / &&

Some differences:
* The `&` version of AND evaluates AND across an entire vector, while the `&&` version of AND only evaluates the first member of a vector.
```
> TRUE & c(TRUE, FALSE, FALSE)
[1]  TRUE FALSE FALSE
```
```
> TRUE && c(TRUE, FALSE, FALSE)
[1] TRUE
```
* The `|` version of OR evaluates OR across an entire vector, while the `||` version of OR only evaluates the first member of a vector.
```
> TRUE | c(TRUE, FALSE, FALSE)
[1] TRUE TRUE TRUE
```
```
> TRUE || c(TRUE, FALSE, FALSE)
[1] TRUE
```

Go to: [R Programming (repository)](https://github.com/bea314/datasciencecoursera/tree/main/2_R%20Programming)  
Go to: [R Programming - week1 (repository)](https://github.com/bea314/datasciencecoursera/tree/main/2_R%20Programming/week%201)

## Contributors
Date | FirstName | LastName | Email
--- | --- | --- | ---
13/12/2020 | Beatriz |  Del Pinal |  <beatrizdelpinal@gmail.com>
--/--/---- | Submit |  Pull Request | <youremailhere@gmail.com>
