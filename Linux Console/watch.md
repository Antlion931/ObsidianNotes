[[watch]] is an program that will run endlessly other command with some delay between.

## Example 

> watch ping google.com -c 1

It will ping google once, wait 2 second, and ping it again, forever.
It is important to use `-c 1` with [[ping]], because [[watch]] will wait until commend ends.