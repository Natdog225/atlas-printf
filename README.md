<a href="https://imgflip.com/i/8vmjky"><img src="https://i.imgflip.com/8vmjky.jpg" title="made at imgflip.com"/></a></div>

# Custom `_printf` Function

This project implements a simplified version of the standard `printf` function in C. The custom `_printf` function provides basic formatted output capabilities and handles the following conversion specifiers: `%c`, `%s`, `%d`, and `%%`.

## Table of Contents

- [Overview](#overview)
- [Requirements](#requirements)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Tasks](#Tasks)
- [Prototypes](#Prototypes)
- [Authors](#Authors)

## Overview

The `_printf` function is a custom implementation of the C standard library function `printf`. It allows you to print formatted output to the standard output stream (stdout). This project is part of a C programming course and aims to demonstrate an understanding of variadic functions and formatted output.

## Requirements

- Allowed editors: `vi`, `vim`, `emacs`
- All files will be compiled on Ubuntu 20.04 LTS using `gcc`, with the options `-Wall -Werror -Wextra -pedantic -std=gnu89`
- All files should end with a new line
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should use the Betty style. It will be checked using `betty-style.pl` and `betty-doc.pl`
- You are not allowed to use global variables
- No more than 5 functions per file
- The prototypes of all your functions should be included in your header file called `main.h`
- All header files should be include guarded
- Authorized functions and macros: `write`, `malloc`, `free`, `va_start`, `va_end`, `va_copy`, `va_arg`

## Project Structure

The project consists of the following files:

- `main.h`: Header file containing function prototypes and necessary includes.
- `_printf.c`: Contains the main `_printf` function which handles the variable arguments and directs them to the appropriate handler functions.
- `format_specifiers.c`: Contains helper functions for handling specific format specifiers (`%c`, `%s`, `%d`).
- `utils.c`: Contains the `_putchar` function used to write characters to the standard output.
- `README.md`: Documentation for the project.
- `test/main.c`: Test file to verify the implementation of the `_printf` function.

## Usage

To use the custom `_printf` function, follow these steps:

1. Include the `main.h` header file in your source file.
2. Compile your source file with the provided `_printf` implementation files.
3. Call the `_printf` function in your code as you would with the standard `printf`.

## Tasks

### Requirements
#### General
- Editors Allowed: vi, vim, emacs
- Compilation: Files will be compiled on Ubuntu 20.04 LTS using gcc with the options -Wall -Werror -Wextra -pedantic -std=gnu89
- End of File: All files should end with a new line
- README.md: A README.md file at the root of the project folder is mandatory
- Code Style: Your code should use the Betty style, checked with betty-style.pl and betty-doc.pl
- Global Variables: Not allowed
- Functions per File: No more than 5 functions per file
- Main Files: Example main.c files are provided for testing but should not be pushed to the repo
- Function Prototypes: Should be included in a header file named main.h
- Header Guards: All header files should be include guarded
- _putchar Function: Not provided for this project
- Compilation
Your code will be compiled with:

- bash
- Copy code
 - $ gcc -Wall -Werror -Wextra -pedantic -std=gnu89 -Wno-format *.c
- Main Files: Our main files will include your main header file (main.h): #include main.h
- Testing with _printf: Use the -Wno-format flag when testing with your _printf and the standard printf
#### Tasks
##### 0. I'm not going anywhere. You can print that wherever you want to. I'm here and I'm a Spur for life.
Write a function that produces output according to a format.

Prototype: int _printf(const char *format, ...);
Returns: The number of characters printed (excluding the null byte used to end output to strings)
Output: Write output to stdout, the standard output stream
Format String: The format string is composed of zero or more directives (See man 3 printf for more detail)
Conversion Specifiers: Handle the following conversion specifiers:
- c
- s
- %
Buffer Handling: No need to reproduce the buffer handling of the C library printf function
Flags, Field Width, Precision, Length Modifiers: No need to handle these.

##### 1. Education is when you read the fine print. Experience is what you get if you don't
Handle the following conversion specifiers:

Conversion Specifiers:
- d
- i
- Flags, Field Width, Precision, Length Modifiers: No need to handle these
##### 2. Just because it's in print doesn't mean it's the gospel
Create a man page for your function.

## Prototypes

This is the putchar function that prints a character.

	int _putchar(char c);

This is the main code that will print things.

	int _printf(const char *format, ...);

This is the helper to handle printing calling a char.

	int handle_char(va_list args);
	
This is the helper to handle printing strings and digits.

	int handle_string(va_list args);

This is the helper to handle printing int's.

	int handle_int(va_list args);
	
This is the helper to handle blank spaces.

	int handle_r(va_list args);

> "Got a long list of ex-lovers, they'll tell you I'm insane, but I've got a blank space, baby, and I'll write your name."
> - Taylor Swift, (probably)

## Authors

- John Wilson
- Nathan Wilson