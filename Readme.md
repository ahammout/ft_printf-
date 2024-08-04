# ft_printf

## Introduction

The `ft_printf` project is a part of the curriculum at 42 school. It aims to reimplement the standard C library function `printf`, which is used to print formatted output to the standard output.

## Features

The mandatory part of this project includes the following features:

- Handling of the following conversions: `c`, `s`, `p`, `d`, `i`, `u`, `x`, and `X`.
- Handling of the `%%` conversion.
- Implementation of the `ft_printf` function with the following prototype:

```c
int ft_printf(const char *format, ...);
```

## Supported Conversion Specifiers

+ %c - Character
+ %s - String
+ %p - Pointer address
+ %d - Decimal (base 10) integer
+ %i - Integer
+ %u - Unsigned decimal (base 10) integer
+ %x - Unsigned hexadecimal (base 16) integer (lowercase)
+ %X - Unsigned hexadecimal (base 16) integer (uppercase)
+ %% - Percent sign

## Usage
To use the ft_printf function in your project, include the ft_printf.h header file and link against the compiled library.

```c
#include "ft_printf.h"

int main(void) {
    ft_printf("Hello, %s!\n", "world");
    return 0;
}
```

## Installation
Clone the repository:

```bash
git clone https://github.com/your-username/ft_printf.git
cd ft_printf
```

Compile the library:

```bash
    make
```

Include ft_printf.h in your project and link the compiled library.

## Examples
```c
ft_printf("Character: %c\n", 'A');
ft_printf("String: %s\n", "Hello, world!");
ft_printf("Pointer: %p\n", (void *)0x7ffee631d1a0);
ft_printf("Decimal: %d\n", 42);
ft_printf("Integer: %i\n", -42);
ft_printf("Unsigned: %u\n", 42);
ft_printf("Hexadecimal (lowercase): %x\n", 255);
ft_printf("Hexadecimal (uppercase): %X\n", 255);
ft_printf("Percent sign: %%\n");
```

