<p align="center">
  <img width="409" height="128" src="https://www.alxafrica.com/wp-content/uploads/2022/01/header-logo.png">
</p>

# An Alternative implementation of printf

This project repository contains an implimentation of the **printf()** function. 

Course: ALX Software Engineering program.

Module: Low level programming.

Project 1: implement printf().

## Project overview

All coding done using Betty coding style

### Flow Diagram
![Example Flowchart](/images/flow.jpg)

### Authorized functions and macros

* write (man 2 write)
* malloc (man 3 malloc)
* free (man 3 free)
* va_start (man 3 va_start)
* va_end (man 3 va_end)
* va_copy (man 3 va_copy)
* va_arg (man 3 va_arg)
* _putchar(char c)

## Function prototypes

All function prototypes used to compile _printf() are included in the header file **holberton.h**:
*    int (*get_func(const char *format))(va_list);
*    int _putchar(char c);
*    int _printf(const char *format, ...);
*    int print_str(va_list args);
*    int print_char(va_list args);
*    int print_pct(va_list args);
*    int print_dec(va_list args);

___

**int (\*get_Specifier_func(const char \*format))(va_list)**

Called to check specifier and return the corresponding print function
___

**int print_dec(va_list args)**

prints integer
___

**int print_char(va_list args)**

Prints Characters 
___

**int print_str(va_list args)**

Prints char of a string one at a time 
___

**int print_pct(va_list args)**

Prints percentage sign
___

**int _putchar(char c)**

writes char to stdout
___

The **conversion specifier:**

**d:**	   decimal.

**i:**	   integer.

**c:**	   character.

**s:**	   string.

**%:**	   Percent.

**Return value:**

Upon success, _printfs return the number of characters printed
A negative 1 is returned on error is.

## Samples:

```c
_printf("Your character is: %c\n", 'H');
Output:   Your character is: K
```
```c
_printf("Your string is: %s\n", "Mpho Kyle");
Output:    Your string is: Mpho Kyle
```
```c
 _printf("Your integer is: %d\n", 2);
Output:   Your integer is: 2
```

## Author(s)
##### Kyle Stols
##### Mpho Chepape
ALX Software Engineering
