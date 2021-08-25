---
Title: "Strings"
Subjects:
  - "Computer Science"
  - "Game Development"
Tags: 
  - "Strings"
  - "Characters"
  - "Data Types"
CatalogContent:
  - "learn-c-plus-plus"
  - "paths/computer-science"
---

Strings are objects that represent sequences of characters. In C++, there are two ways to create strings: `string` class or using C-style character strings.

## String Class

The standard `string` class provides support for strings in C++.

```cpp
std::string welcome = "Hi";
std::string user_name = "@sonny";
std::string message = "Good nite! 😇";
```

## C-Style Character Strings

The C-style character string originated from the C language and continues to be supported within C++. 

In C, the string is actually an array of characters, followed by a `null` character `'\0'`.

```cpp
char greeting[] = "Hello";
```

So here's the memory presentation:

```shell
Character |   'H'    'e'    'l'    'l'    'o'   '\0'
Index     |    0      1      2      3      4      5
Address   |  23451  23452  23453  23454  23455  23456
```
