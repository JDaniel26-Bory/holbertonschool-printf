<p align="center">
<img src="https://www.freepik.com/free-photo/it-specialist-checking-code-computer-dark-office-night_5698336.htm#query=development&from_query=develoment&position=23&from_view=search&track=sph" width="450" height="250">	
<h1> Printf project </h1></p>

<h3> Description</h3>
<p>printf is a weel known function used in C programming to do formated printing. Usually it only takes the standard library 
<stdio.h> to call it into a c program, and using it for simple strings or formatted specifiers that allow us to print diferent types of data. This time we are presenting a printf project made from scratch in most of its features in order to understand the complexity of a powerful tool. You can see man 3 of printf to understand how _printf works.</p>

<h3> Compilation</h3>

```$ gcc -Wall -Werror -Wextra -pedantic *.c```


<h3> Prototype </h3>

```int _printf(const char *format, ...)```


<h3>Return</h3>
If everything is succesful the function returns the number of characteres printed.

<h3>Formats</h3>

| Specifiers      | Description |
| ----------- | ----------- |
| %c  | Print single character |
| %s  | Print string of characteres |
| %d  | Print decimal numbers|
| %i  | Print integers |

<h3>Project files</h3>

 File        | Description |
| ----------- | ----------- |
| [main.h](https://github.com/JDaniel26-Bory/holbertonschool-printf/blob/main/main.h)                | **Header file**<br>Include all  function prototypes<br> Include structure of specifiers|
| [printf.c](https://github.com/JDaniel26-Bory/holbertonschool-printf/blob/main/printf.c)                      | **Project function: _printf** <br> Start the variadic list.<br> Iterates string  format  of entry and check for a moldule symbol (%) . If  the symbol is found then check if the next char match with one of the valid specifiers in the structure using the auxiliar function to comapare ( comp), in that case the respective function of these format is called.<br> For the characters that doesn't match any of the formats the function ignores the module symbole and print it  as a string.<br> In case that  the module symbole is not found, print the each character normally.|
| [printf_functions.c](https://github.com/JDaniel26-Bory/holbertonschool-printf/blob/main/printf_functions.c)  | **Auxiliar functions**<br> _putchar: using write function, prints a character<br> printc: print character using list variable.<br> print_string: print <strings, if string is null it pirnts (null)<br> print_n: print numbers base 10.|
| [printf_functions.c](https://github.com/JDaniel26-Bory/holbertonschool-printf/blob/main/man_3_printf)  | **Man Of our Re-creation of pritf**<br>man_3_printf: The structure of a man page Man pages are all laid out with specific sections, which include: NAME - the name of the command in questio.
SYNOPSIS - the structure of the command.
DESCRIPTION - a description of the command.
OPTIONS - available options for the command.
AUTHOR - the author of the command.
REPORTING BUGS - instructions on reporting bugs to the developer(s).
COPYRIGHT - information about command license.
SEE ALSO - points to full documentation or related commands.
CONFIGURATION - configuration details for a command or device.
EXIT STATUS - possible exit status values.|

<h3>Contributors</h3>

Juan Daniel Restrepo - [@JDaniel26-Bory](https://github.com/JDaniel26-Bory)<br>
Ruben Dario Florez - [@Rubio91147](https://github.com/Rubio91147)<br>
