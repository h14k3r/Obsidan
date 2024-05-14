# what is it

Allows an attacker to read files on the server that is running the application.
- uses GET requests to get the data you ask for, such as a cat picture: www.random.com/images?filename=cat.png

Example of attack:
> https://www.random.com/images?filename=/etc/passwd


# how to find
Code Review:
> <?php
> $template = 'blue.php'
> if ( is_set ( $_COOKIE['TEMPLATE'] ) )
>   $template = $_COOKIE['TEMPLATE'];
> include ( "/home/users/phpguru/templates/" . $template );
> ?>

# how to exploit


# how to prevent

