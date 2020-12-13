# Week 1 Quiz

Go to: [R Programming (repository)](https://github.com/bea314/datasciencecoursera/tree/main/2_R%20Programming)  
Go to: [R Programming - week1 (repository)](https://github.com/bea314/datasciencecoursera/tree/main/2_R%20Programming/week%201)

## Question 1
1. R was developed by statisticians working at
- [ ] Harvard University
- [x] The University of Auckland
- [ ] Bell Labs
- [ ] StatSci

## Question 2
2. The definition of free software consists of four freedoms (freedoms 0 through 3). Which of the following is NOT one of the freedoms that are part of the definition? Select all that apply.
- [ ] The freedom to study how the program works, and adapt it to your needs.
- [x] The freedom to sell the software for any price.
- [ ] The freedom to run the program, for any purpose.
- [x] The freedom to restrict access to the source code for the software.
- [ ] The freedom to redistribute copies so you can help your neighbor.
- [ ] The freedom to improve the program, and release your improvements to the public, so that the whole community benefits.
- [x] The freedom to prevent users from using the software for undesirable purposes.

## Question 3
3. In R the following are all atomic data types EXCEPT: (Select all that apply)
- [x] data frame
- [ ] logical
- [x] matrix
- [ ] complex
- [ ] character
- [x] list
- [x] array
- [ ] numeric
- [x] table
- [ ] integer

## Question 4
4. If I execute the expression x <- 4 in R, what is the class of the object 'x' as determined by the 'class()' function?
- [x] numeric
- [ ] complex
- [ ] integer
- [ ] vector
- [ ] matrix
- [ ] real
- [ ] list

Code:
```
    x <- 4
    x
    class(x)
```
Result:
```
     [1] 4
     [1] "numeric"
```

## Question 5
5. What is the class of the object defined by x <- c(4, TRUE)?
- [ ] list
- [ ] logical
- [x] numeric
- [ ] integer
- [ ] matrix
- [ ] character

Code:
```
    x <- c(4, TRUE)
    class(x)
```
Result:
```
    [1] 4 1
    [1] "numeric"
```

## Question 6
6. If I have two vectors x <- c(1,3, 5) and y <- c(3, 2, 10), what is produced by the expression cbind(x, y)?
- [ ] a vector of length 2
- [ ] a 3 by 3 matrix
- [ ] a 2 by 3 matrix
- [ ] a vector of length 3
- [ ] a 2 by 2 matrix
- [x] a matrix with 2 columns and 3 rows

Code:
```
    x <- c(1,3, 5)
    y <- c(3, 2, 10)
    cbind(x, y)
```
Result:
```
         x  y
    [1,] 1  3
    [2,] 3  2
    [3,] 5 10
```

## Question 7
7. A key property of vectors in R is that
- [x] elements of a vector all must be of the same class
- [ ] elements of a vector can only be character or numeric
- [ ] elements of a vector can be of different classes
- [ ] a vector cannot have have attributes like dimensions
- [ ] the length of a vector must be less than 32,768

## Question 8
8. Suppose I have a list defined as x <- list(2, "a", "b", TRUE). What does x[[2]] give me? Select all that apply.
- [x] a character vector of length 1.
- [ ] a list containing character vector with the letter "a".
- [ ] a list containing a character vector with the elements "a" and "b".
- [x] a character vector containing the letter "a".
- [ ] a character vector with the elements "a" and "b".

Code:
```
    x <- list(2, "a", "b", TRUE)
    a <- x[[2]]
    a
    class(a)
```
Result:
```
    [1] "a"
    [1] "character"
```

OR

8. Suppose I have a list defined as x <- list(2, "a", "b", TRUE). What does x[[1]] give me? Select all that apply.
- [ ] a list containing the number 2.
- [ ] a list containing a numeric vector of length 1.
- [x] a numeric vector of length 1.
- [ ] a character vector containing the element "2".
- [x] a numeric vector containing the element 2.

## Question 9
9. Suppose I have a vector x <- 1:4 and a vector y <- 2. What is produced by the expression x + y?
- [ ] a numeric vector with elements 1, 2, 3, 6.
- [ ] an integer vector with elements 3, 2, 3, 6.
- [ ] a numeric vector with elements 3, 2, 3, 6.
- [x] a numeric vector with elements 3, 4, 5, 6.
- [ ] a numeric vector with elements 3, 2, 3, 4.
- [ ] an integer vector with elements 3, 2, 3, 4.

Code:
```
    x <- 1:4
    y <- 2
    a <- x + y
    a
    class(a)
```
Result:
```
    [1] 3 4 5 6
    [1] "numeric"
```

OR

9. Suppose I have a vector x <- 1:4 and y <- 2:3. What is produced by the expression x + y?
- [ ] a numeric vector with the values 1, 2, 5, 7.
- [ ] an error.
- [ ] an integer vector with the values 3, 5, 3, 4.
- [ ] an numeric vector with the values 3, 5, 5, 7.
- [ ] a warning
- [x] an integer vector with the values 3, 5, 5, 7.

## Question 10
10. Suppose I have a vector x <- c(3, 5, 1, 10, 12, 6) and I want to set all elements of this vector that are less than 6 to be equal to zero.
What R code achieves this? Select all that apply.
- [ ] x[x == 0] < 6
- [ ] x[x == 0] < 6
- [ ] x[x > 6] <- 0
- [ ] x[x < 6] == 0
- [ ] x[x > 0] <- 6
- [x] x[x < 6] <- 0
- [x] x[x <= 5] <- 0
- [ ] x[x >= 6] <- 0
- [ ] x[x != 6] <- 0
- [x] x[x %in% 1:5] <- 0
- [ ] x[x == 6] <- 0
- [ ] x[x == 0] <- 6

## Question 11
11. Use the Week 1 Quiz Data Set to answer questions 11-20. In the dataset provided for this Quiz, what are the column names of the dataset?
- [ ] 1, 2, 3, 4, 5, 6
- [ ] Month, Day, Temp, Wind
- [ ] Ozone, Solar.R, Wind
- [x] Ozone, Solar.R, Wind, Temp, Month, Day

Code:
```
    data <- read.csv("hw1_data.csv")
    # OR
    data <- read.table("hw1_data.csv", header = TRUE, sep = ",", stringsAsFactors = FALSE)
```
Result:
```
        Ozone Solar.R Wind Temp Month Day
    1      41     190  7.4   67     5   1
    2      36     118  8.0   72     5   2
    3      12     149 12.6   74     5   3
    4      18     313 11.5   62     5   4
    5      NA      NA 14.3   56     5   5
    6      28      NA 14.9   66     5   6
    # continue...
```

## Question 12
12. Extract the first 2 rows of the data frame and print them to the console. What does the output look like?
- [ ] Option 1

*| Ozone | Solar.R | Wind | Temp | Month | Day
--- | --- | --- | --- | --- | --- | ---
1 | 18 | 224 | 13.8 | 67 | 9 | 17
2 | NA | 258 | 9.7 | 81 7 | 22

- [ ] Option 2

*| Ozone | Solar.R | Wind | Temp | Month | Day
--- | --- | --- | --- | --- | --- | ---
1 | 924 | 10.9 | 71 | 9 | 14
2 | 18 | 131 | 8.0 | 76 | 9 | 29

- [x] Option 3

*| Ozone | Solar.R | Wind | Temp | Month | Day
--- | --- | --- | --- | --- | --- | ---
1 | 41 | 190 | 7.4 | 67 | 5 | 1
2 | 36 | 118 | 8.0 | 72 | 5 | 2

- [ ] Option 4

*| Ozone | Solar.R | Wind | Temp | Month | Day
--- | --- | --- | --- | --- | --- | ---
1 | 7 | NA | 6.9 | 74 | 5 | 11
2 | 35 | 274 | 10.3 | 82 | 7 | 17


## Question 13
13. How many observations (i.e. rows) are in this data frame?
- [ ] 160
- [ ] 129
- [x] 153
- [ ] 45

Code:
```
    nrow(data)
```
Result:
```
    [1] 153
```

## Question 14
14. Extract the last 2 rows of the data frame and print them to the console. What does the output look like?
- [x] Option 1

*| Ozone | Solar.R | Wind | Temp | Month | Day
--- | --- | --- | --- | --- | --- | ---
152 | 18 | 131 | 8.0 | 76 | 9 | 29
153 | 20 | 223 | 11.5 | 68 | 9 | 30

- [ ] Option 2

*| Ozone | Solar.R | Wind | Temp | Month | Day
--- | --- | --- | --- | --- | --- | ---
152 | 31 | 244 | 10.9 | 78 | 8 | 19
153 | 29 | 127 | 9.7 | 82 | 6 | 7

- [ ] Option 3

*| Ozone | Solar.R | Wind | Temp | Month | Day
--- | --- | --- | --- | --- | --- | ---
152 | 11 | 44 | 9.7 | 62 | 5 | 20
153 | 108 | 223 | 8.0 | 85 | 7 | 25

- [ ] Option 4

*| Ozone | Solar.R | Wind | Temp | Month | Day
--- | --- | --- | --- | --- | --- | ---
152 | 34 | 307 | 12.0 | 66 | 5 | 17
153 | 13 | 27 | 10.3 | 76 | 9 | 18

Code:
```
    tail(data, 2)
    # OR
    x <- data[c(nrow(data)-1,nrow(data)),]
```

## Question 15
15. What is the value of Ozone in the 47th row?
- [ ] 34
- [ ] 63
- [ ] 18
- [x] 21

Code:
```
    data[47, "Ozone"]
```

## Question 16
16. How many missing values are in the Ozone column of this data frame?
- [ ] 43
- [x] 37
- [ ] 78
- [ ] 9

Code:
```
    data <- read.csv("hw1_data.csv")
    sum(is.na(data$Ozone))
    # OR
    # gives a summary of the matrix
    summary(data)
    # OR (better if column)
    # gives the quantity of each number in the column
    table(z$Ozone, exclude=NULL)
    # OR
    # creates a matrix only with the rows with NA values
    sub = subset(data, is.na(Ozone))
    nrow(sub)
```

## Question 17
17. What is the mean of the Ozone column in this dataset? Exclude missing values (coded as NA) from this calculation.
- [ ] 18.0
- [x] 42.1
- [ ] 31.5
- [ ] 53.2

Code:
```
    data <- read.csv("hw1_data.csv")
    # gives a summary of the matrix
    summary(data)
    # OR
    sub = subset(data, !is.na(Ozone))
    colMeans(sub)
    # OR
    # just for ozone
    sub = subset(data, !is.na(Ozone),select = Ozone)
    apply(sub, 2, mean) 
```

## Question 18
18. Extract the subset of rows of the data frame where Ozone values are above 31 and Temp values are above 90. What is the mean of Solar.R in this subset?
- [ ] 334.0
- [ ] 205.0
- [x] 212.8
- [ ] 185.9

Code:
```
    data <- read.csv("hw1_data.csv")
    sub = subset(data, Ozone > 31 & Temp > 90,select = Solar.R)
    summary(sub)
    # OR
    colMeans(sub)
    # OR
    apply(sub, 2, mean) 
```

## Question 19
19. What is the mean of "Temp" when "Month" is equal to 6?
- [x] 79.1
- [ ] 90.2
- [ ] 85.6
- [ ] 75.3

Code:
```
    data <- read.csv("hw1_data.csv")
    sub = subset(data, Month == 6, select = Temp)
    summary(sub)
    # OR
    colMeans(sub)
    # OR
    apply(sub, 2, mean) 
```

## Question 20
20. What was the maximum ozone value in the month of May (i.e. Month is equal to 5)?
- [x] 115
- [ ] 97
- [ ] 100
- [ ] 18

Code:
```
    data <- read.csv("hw1_data.csv")
    sub = subset(data, Month == 5, select = Ozone)
    summary(sub)
    # OR
    sub = subset(data, !is.na(Ozone) & Month == 5, select = Ozone)
    apply(sub, 2, max) 
```

## Resources
[Link 1](https://discuss.analyticsvidhya.com/t/how-to-count-the-missing-value-in-r/2949)  
[Link 2](https://github.com/mGalarnyk/datasciencecoursera/blob/master/2_R_Programming/quizzes/quiz1.md)  
[Link 3](https://www.geeksforgeeks.org/calculate-the-mean-of-each-column-of-a-matrix-or-array-in-r-programming-colmeans-function/)

## Contributors
Date | FirstName | LastName | Email
--- | --- | --- | ---
12/12/2020 | Beatriz |  Del Pinal |  <beatrizdelpinal@gmail.com>
--/--/---- | Submit |  Pull Request | <youremailhere@gmail.com>
