# Module 2: Data types, variables, input-output operations and operators

### Where functions come from
Built in
Modules
Written by programer

### The print() function
* Can have none or n arguments.
* Accepts the following two kwargs: "end=" to define the last character of the print, and "sep=" to set the character that separates each argument to be printed.
* By default end=\n and sep=" "
* Accepts all types of data offered by Python as argument
* An empty print() outputs a line

### Backslash \
* Is a special character that announces about the next character having a special meaning.

### Positional arguments


### Literal
* Is the data itself, like a string "123" or an integer 25.

### Integers
* Are numbers devoided of the fractional part.
* The same integer can have different representations like: 11111 == 11_11_1 and -222222 == -222_222

### Floats
* Numbers that contain the fractional part.
* The same float number can have different representations like: 0.4 is the same as .4 and 4.0 is the same as 4.

### Integer x Float
* They differ on how they are stored in memory.

### Octal numbers
* Represented by 0o or 0O .

### Hexadecimal
* Represented by Ox or OX .

### Scientific notation
* 3x10ˆ8 is represented by 3E8 .
* The base of the representation may be an integer and the exponent has to be integer.

### Strings
* When necessary to use apostrophes or quotes inside a string this is possible using the scape character "text \"text\"".


### String operators
* Concatenation is done by the + sing and both arguments must be string: "text" + "text".
* Replication is done by de * sign and the arguments must be a number and a string: "text" * 3 or 5 * "text". If the number is <=1 the result is an empty string "".


### Operators
* Exponential ** conforms to the integer vs. float rule. Uses right-sided binding.
* Multiplication * conforms to the integer vs. float rule
* Division / the result is always a float.
* Integer Division (floor division) // it conforms to the integer vs. float rule. The result ignores the fractional part and it is rounded toward the lesser integer value. Ex.: -6//4 = -2
* Remainder % the result conforms to the integer vs. float rule


### Variables
* Variable names rules: 
    ** must begin with a letter or underscore
    ** python is case sensitive 
    ** can have letters, digits, and the character underscore
* According to PEP functions and variables names should have words separated by underscores.

### Shortcut operators
You can substitute the expressions like:
```
var = var op expression 
```
By:
```
var op = expression
```
Ex
```
var /= 5 * 2
```

### Multiple lines comment
They have the following syntax:
```
'''
Comment
'''
```

### The input() function
* Changes the console to input mode and the data inputted is received by the program.
* The result is always a STRING and must be assigned to a variable so the data isn't lost.
* The function can be invoked with none or one argument.

### Type casting
* int() to convert string to a number.
* float() to convert string to a number.
* string() to convert number to a string.
