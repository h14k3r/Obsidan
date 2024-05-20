Resource: Rana Khalil
Link: https://academy.ranakhalil.com/courses/1491236/lectures/44691833

# what is it

Allows an attacker to read files on the server that is running the application.
- uses GET requests to get the data you ask for, such as a cat picture: www.random.com/images?filename=cat.png

Example of attack:
> https://www.random.com/images?filename=/etc/passwd


# how to find
Code Review:

```
 <?php
$template = 'blue.php'
if ( is_set ( $_COOKIE['TEMPLATE'] ) )
	$template = $_COOKIE['TEMPLATE'];
 include ( "/home/users/phpguru/templates/" . $template );
?> 
```

Line: 20 ( include line ) is the issue:
> evaluates a file path that is taken from user supplied input.






# how to exploit

Example:

```
GET /vulnerable.php HTTP/1.0
Cookie: TEMPLATE=../../../../../etc/passwd
```


# how to prevent

( here there is no proper validation in the user input )