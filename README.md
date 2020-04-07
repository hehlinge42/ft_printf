# ft_printf @42

This project aims at coding a library providing the *ft_printf* function, that imitates printf's behavior.

## Installation

In a UNIX terminal, type the command line `gcl https://github.com/hehlinge42/ft_printf.git`
Enter the ft_printf repository by typing `cd ft_printf`
Compile the project by typing `make`. It generates the library *libftprintf.a*

## Format

Like *printf*, format for *ft_printf* is *%[flags][width][.precision][size]type*

## Supported features

### Types

It displays the following types:
- `%c`: displays a character (type *char*)
- `%s`: displays a string (type *char \**)
- `%p`: displays an address in memory in hexadecimal (format 0xffffffff)
- `%d` and `%i`: display a integer
- `%u`: displays an unsigned integer
- `%o`: displays an unsigned integer in the octal base
- `%x` and `%X`: display an integer in the hexadecimal base
- `%f`: displays a float number

### Type modifiers

It supports the following type modifiers:
- `hh`: indicates that the following integer is of type *char*
- `h`: indicates that the following is of type *short*
- `l`: indicates that the following integer is of type *long* or that the following float is of type *double*
- `ll`: indicates that the following integer is of type *long long*
- `L`: indicates that the following float is of type *long double*

### Flags

It supports the following flags:
- `#`: for o conversions, the flag prepends the number by a `0`. For x and X conversions, a non-zero result has the string `0x' (or `0X' for X conversions) prepended to it.
- `0`: The converted value is padded on the left with zeros rather than blanks. If a precision is given with a numeric conversion (d, i, o, u, i, x, and X), the 0 flag is ignored.
- `-`: the converted value is padded on the right with blanks, rather than on the left with blanks or zeros.  A - overrides a 0 if both are given.
- `space`: A blank should be left before a positive number produced by a signed conversion
- `+`: A sign must always be placed before a number produced by a signed conversion.  A + overrides a space if both are used.

### Width and precision

It supports width and precision.
It supports the escaper `%%`



