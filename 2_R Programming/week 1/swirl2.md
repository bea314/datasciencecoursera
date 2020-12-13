# 2. Workspace and Files

Commands:
* Determine which directory your R session is using as its current working directory:  
```getwd()```

* List all the objects in your local workspace:  
```ls()```

* List all the files in your working directory:
```dir()```

* Using the args() function on a function name is also a handy way to see what arguments a function can take:  
```args()```

* Create a directory in the current working directory:  
```dir.create()```  
```setwd()```

* Create a file in your working directory:  
```file.create()```

* Access information about a file:  
```file.info()```

You can use the $ operator --- e.g., file.info("mytest.R")$mode --- to grab specific items.

* Change the name of the file:
```file.rename()```

* Delete file:
```file.remove()```

* Make a copy of a file:
```file.copy()```

* Provide the relative path to a file. Construct file and directory paths that are independent of the operating system your R code is running on. 
```file.path()```

Go to: [R Programming (repository)](https://github.com/bea314/datasciencecoursera/tree/main/2_R%20Programming)  
Go to: [R Programming - week1 (repository)](https://github.com/bea314/datasciencecoursera/tree/main/2_R%20Programming/week%201)

## Contributors
Date | FirstName | LastName | Email
--- | --- | --- | ---
12/12/2020 | Beatriz |  Del Pinal |  <beatrizdelpinal@gmail.com>
--/--/---- | Submit |  Pull Request | <youremailhere@gmail.com>
