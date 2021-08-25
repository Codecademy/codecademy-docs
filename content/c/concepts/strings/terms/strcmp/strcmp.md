---
Title: "strcmp()"
Description: "Compares two strings."
Subjects:
  - "Code Foundations"
  - "Computer Science"
Tags: 
  - "Strings"
  - "Data Types"
  - "Characters"
  - "Arrays"
  - "Functions"
CatalogContent:
  - "learn-c-plus-plus"
  - "paths/computer-science"
---

The `strcmp()` string function compares two strings and returns an integer value.

## Syntax

```c
strcmp(string1, string2)
```

- If the two strings are same, return 0.
- If `string1` > `string2`, return positive value.
- If `string1` < `string2` or `string1` is a substring of `string2`, return negative value. 

## Example

```c
#include <stdio.h>
#include <string.h>

int main() {
  char address1[20] = "575 Broadway";
  char address2[20] = "576 Broadway";

  if (strcmp(address1, address2) == 0) {
    printf("Address 1 and address 2 are equal.");
  } 
  else {
    printf("Address 1 and address 2 are different.");
  }
  return 0;
}
```
