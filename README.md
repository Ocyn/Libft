<br/>
<p>
  <a href="https://github.com/Ocyn/Libft">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8d/42_Logo.svg/768px-42_Logo.svg.png" alt="Logo" width="80" height="80">
  </a>

  <h1>Libft</h1>

  <p>
    42 School Project | Made in 2023 - 2024
    <br/>
    <br/>
  </p>
</p>

![Contributors](https://img.shields.io/github/contributors/Ocyn/Libft?color=dark-green) ![Issues](https://img.shields.io/github/issues/Ocyn/Libft) ![License](https://img.shields.io/github/license/Ocyn/Libft) 

## Table Of Contents

* [About the Project](#about-the-project)
* [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Usage](#usage)
* [Authors](#authors)
* [Acknowledgements](#acknowledgements)

## About The Project

Libft is a comprehensive C library that provides a set of essential functions for string manipulation, memory management, and character checking. The library includes functions like ft_atoi, ft_bzero, ft_memcpy, and many more, offering a fundamental toolkit for C programming.

The primary goal of this project is to create a personal library of useful functions that students can use in various 42 School projects. By implementing these functions from scratch, participants gain a deeper understanding of how standard C library functions work. Additionally, the Makefile provided simplifies the compilation process, allowing users to create the libft.a library effortlessly.

To use this library, simply include the "libft.h" header file in your C projects and link against the libft.a archive. The Makefile facilitates compilation, making it easy to integrate the libft functions into your 42 School assignments.

## Built With



* [C](https://en.wikipedia.org/wiki/C_(programming_language))

## Getting Started

**Compatibility Warning**

This project, Libft, has primarily been developed and tested on a Linux Ubuntu system. It is essential to note that the project may encounter compatibility issues when executed on different operating systems. The utilization of Linux-specific features, libraries, or commands could lead to unexpected behavior on non-Linux platforms.

To ensure optimal performance and compatibility, it is recommended to run this project on a Linux environment, preferably Ubuntu. Attempting to execute the project on other operating systems may result in errors or unintended behavior.

Please consider this compatibility notice before proceeding with the compilation and execution of Libft.

### Prerequisites

If you don't have Make
* Make

```sh
apt-get install build-essential make
```

### Installation

Clone the repo

```sh
git clone https://github.com/Ocyn/Libft.git
cd Libft/
```

**Make options**
- Compile
```sh
Make
```
- Clear .o files
```sh
Make clean
```
- Clear all (.o files and .a library)
```sh
Make fclean
```
- Re-compile (clear all and compile)
```sh
Make re
```

## Usage

The LIBFT library is a C library developed as part of a project at 42 School. Its purpose is to provide students with a collection of basic functions commonly used in C programming. By implementing these functions from scratch, students gain a deep understanding of their internal workings.

Here's how to use the LIBFT library in your C projects:

Include the Header File (libft.h):
Make sure to include the libft.h header file at the beginning of your program or source file. This allows access to the prototypes of all functions provided by the library.
```c
#include "libft.h"
```

Compile the Library:
Compile the library using the provided Makefile. Ensure that the Makefile is in the same directory as your source files. Execute the make command to compile the library.
```bash
make
```
This will create a static file named libft.a containing all the functions from the library.

Link with Your Program:
When compiling your program, make sure to link with the LIBFT library by specifying the path to the libft.a file.
```bash
gcc -o my_program my_program.c -L. -lft
```
Here, -L. specifies that the compiler should look for the library in the current directory, and -lft indicates linking with the libft.a library.

Use LIBFT Functions:
You can now use any function from the LIBFT library in your program. For example, if you want to use the ft_strlen function to calculate the length of a string, call it as follows:

```c
#include "libft.h"

int main(void) {
    char *myString = "Hello, LIBFT!";
    size_t length = ft_strlen(myString);
    printf("Length: %zu\n", length);
    return 0;
}
```
Clean Up:
After finishing, ensure to clean up the generated object files by running make clean, and if necessary, delete the libft.a file with make fclean.
```bash
make clean
```
This will remove the object files created during compilation.

By following these steps, you can integrate and use the functions from the LIBFT library in your C projects at 42 School.

## Authors

* **Ocyn** - *A Random Dev* - [Ocyn](https://github.com/Ocyn) - *Made the project*

## Acknowledgements

* [42 School](https://github.com/42School)
