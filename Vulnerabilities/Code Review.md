# php

#### include
> takes all the data that exists in the specified file and loads it into the memory, to allow it to be used when needed or called.

[[resources_VU]]


Example: 

```
File 1 --> vars.php
<?php
$color = 'green';
$fruit = 'apple';
?>
#############################################
File 2 --> test.php
<?php
echo "A $color $fruit"; // output = "A"
include 'vars.php';
echo "A $color $fruit"; // output = "A green apple"
?>

```


