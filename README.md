<a href="https://imgflip.com/i/8vm2yr"><img src="https://i.imgflip.com/8vm2yr.jpg" title="made at imgflip.com"/></a></div>

# Custom `_printf` Function

This project implements a simplified version of the standard `printf` function in C. The custom `_printf` function provides basic formatted output capabilities and handles the following conversion specifiers: `%c`, `%s`, `%d`, and `%%`.

## Table of Contents

- [Overview](#overview)
- [Requirements](#requirements)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Tasks](#tasks)
- [Authors](#authors)

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

printf (3)
### Requirements
#### General
- Allowed editors: vi, vim, emacs
- All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
- All your files should end with a new line
- A README.md file, at the root of the folder of the project is mandatory
- Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
- You are not allowed to use global variables
- No more than 5 functions per file
- In the following examples, the main.c files are shown as examples. You can use them to test your functions, but you don’t have to push them to your repo (if you do we won’t take them into account). We will use our own main.c files at compilation; do not push your own main.c file. Our main.c files might be different from the one shown in the examples
- The prototypes of all your functions should be included in your header file called main.h
- Don’t forget to push your header file
- All your header files should be include guarded
- Note that we will not provide the _putchar function for this project
#### GitHub
- There should be one project repository per group. If you clone/fork/whatever a project repository with the same name before the second deadline, you risk a 0% score.

#### 0. I'm not going anywhere. You can print that wherever you want to. I'm here and I'm a Spur for life

Write a function that produces output according to a format.

- Prototype: int _printf(const char *format, ...);
- Returns: the number of characters printed (excluding the null byte used to end output to strings)
write output to stdout, the standard output stream format is a character string. The format string is composed of zero or more directives. See man 3 printf for more detail. You need to handle the following conversion specifiers:
- %c
- %s
- %
- You don’t have to reproduce the buffer handling of the C library printf function
- You don’t have to handle the flag characters
- You don’t have to handle field width
- You don’t have to handle precision
- You don’t have to handle the length modifiers
Repo:
GitHub repository: atlas-printf

#### 1. Education is when you read the fine print. Experience is what you get if you don't.

Handle the following conversion specifiers:

- %d
- %i

- You don’t have to handle the flag characters
- You don’t have to handle field width
- You don’t have to handle precision
- You don’t have to handle the length modifiers

Repo:
GitHub repository: atlas-printf

#### 2. Just because it's in print doesn't mean it's the gospel

Create a man page for your function.

Repo:

GitHub repository: atlas-printf
File: man_3_printf

## Authors

- John Wilson
- Nathan Wilson