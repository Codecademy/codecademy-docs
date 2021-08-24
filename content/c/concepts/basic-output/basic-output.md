---
Title: "Basic Output"
Subjects:
  - "Code Foundations"
  - "Computer Science"
Tags:
  - "Print"
  - "Output"
CatalogContent:
  - "learn-c-plus-plus"
  - "paths/computer-science"
---

In the C language basic console output is achieved using functions from the standard input output header file (**stdio.h**)

## Including Output functions

C itself has no ability to output any information, in order to so the **stdio.h** header file must be included in the program, which is typically done at the top of the file.

```c
#include <stdio.h>
```

Once this is done the functions included in it can be used.

## Printing Single Characters With `putchar()`

The `putchar()` function accepts a single `char` input, and prints it to the `stdout` file, normally the console.

```pseudo
#include <stdio.h>

int main(void) {
  putchar('a');
  return 0;
}
```

## Printing Strings With `puts()`

The `puts()` function, or "put string", takes a string as an argument and prints it to the `stdout` file followed by a newline character.

```c
#include <stdio.h>

int main(void) {
  puts("Hello World!!");
  return 0;
}
```

## Formatting Variables With `printf()`

The `puts()` function can only accept and print a single string argument, which is why there is the `printf()` function, or "print formatted". As arguments it takes a string, containing information on what values to format, followed by the values to format in the string.

```c
#include <stdio.h>

int main(void) {
  printf("%d is a number\n", 5); 
  printf("%d is after %d\n, 2, 1);

  return 0;
}
```

```pseudo
5 is a number
2 is after 1
```

As seen above the string given contains a `%` character followed by a letter to indicate what type of value will be formatted there. Some common ones are show below.

```pseudo
%c = char
%d = double
%i = input
%p = pointer
%s = string
```
