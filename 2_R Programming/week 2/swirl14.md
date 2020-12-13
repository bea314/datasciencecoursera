# 8. Logical

R has a special way of representing dates and times, which can be helpful if
you're working with data that show how something changes over time (i.e.
time-series data) or if your data contain some other temporal information, like
dates of birth.

Dates are represented by the 'Date' class and times are represented by the
'POSIXct' and 'POSIXlt' classes. Internally, dates are stored as the number of
days since 1970-01-01 and times are stored as either the number of seconds since
1970-01-01 (for 'POSIXct') or a list of seconds, minutes, hours, etc. (for
'POSIXlt').

### date -- YEAR-MONTH-DAY

Commands:
* Current date:  
  ```Sys.Date()```  
    e.g.   
    d1 <- Sys.Date()
* Assign somde date:  
  ```as.Date()```  
    e.g.  
    d2 <- as.Date("1969-01-01")
* Current date and time:  
  ```Sys.time()```
* Coerce the result of Sys.time to 'POSIXlt':  
  ```as.POSIXlt(Sys.time())```  
* For better visualization of an POSIXlt object:  
  ```str(unclass(t2))```
* Return the day of week from any date or time object:  
  ```weekdays()```
* Return the month from any date or time object:  
  ```months()```
* Returns the quarter of the year (Q1-Q4) from any date or time object.  
  ```quarters()```
* Converts character vectors to POSIXlt, the input doesn't have to be in a particular format (YYYY-MM-DD).  
  ```strptime()```  
    e.g.  
    t3 <- "October 17, 1986 08:24"
* Allows you to specify a 'units' parameter:  
  ```difftime()```
  e.g.  
  difftime(Sys.time(), t1, units = 'days')
  
## Contributors
Date | FirstName | LastName | Email
--- | --- | --- | ---
13/12/2020 | Beatriz |  Del Pinal |  <beatrizdelpinal@gmail.com>
--/--/---- | Submit |  Pull Request | <youremailhere@gmail.com>
