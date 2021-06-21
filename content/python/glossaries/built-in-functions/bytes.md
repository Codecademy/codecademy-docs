---
Title: "bytes()"
Subjects:
  - "Computer Science"
  - "Data Science"
Tags:
  - "Functions"
  - "Methods"
  - "Debugging"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-python-3"
  - "https://www.codecademy.com/learn/paths/computer-science"
  - "https://www.codecademy.com/learn/paths/data-science"
---

## Definition

Returns a byte immutable object representing the given bytes of an object.

## Syntax

```py
bytes(source, encoding, error)
```

## Parameters

* source(optional): specifies the source to initialize the byte represented object.
* encoding(optional): specifies the encoding method of the object.
* errors(optional): specifies the action to take in case of error.


## Example 1

Use `bytes()` to encode the string `"Welcome to Codecademy!"` to unicode `utf-8` and print the number of bytes in the string:

```codebyte/python
print(bytes("Welcome to Codepedia!", "utf-8"))
print(len(bytes("Welcome to Codepedia!", "utf-8")))
```

## Example 2

Use `bytes()` to encode the integer `3`, and print the number of bytes in the integer:

```codebyte/python
print(bytes(5))
print(len(bytes(5)))
```

## Example 3

Use `bytes()` to encode the list of integers `[5, 6, 7]`, and print the number of bytes in the list:

```codebyte/python
grocery_list = [5, 6, 7]

print(bytes(grocery_list))
print(len(bytes(grocery_list)))
```
