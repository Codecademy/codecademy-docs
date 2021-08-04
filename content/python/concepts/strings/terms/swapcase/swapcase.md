---
Title: ".swapcase()"
Description: "Takes a string and returns a copy of that string in which all lowercase letters are uppercase, and all upercase letters are lowercase. Numbers and symbols are not changed."
SUbjects:
  - "Data Science"
  - "Computer Science"
Tags: 
  - "Strings"
  - "Methods"
  - "Functions"
Catalog Content: 
  - "https://www.codecademy.com/learn/learn-python-3"
  - "https://www.codecademy.com/learn/paths/analyze-data-with-python"
---

## Definition 

Takes a string and returns a copy of that string in which all lowercase letters are uppercase, and all upercase letters are lowercase. Numbers and symbols are not changed.

## Syntax

```python
string.swapcase()
```

## Example 1

```python
message = "Hello, World!"

new_string = message.swapcase()

print(new_string)
# Output: "hELLO, wORLD!"
```

## Example 2

The `.swapcase()` method does not change the string it is used on:

```codebyte/py
my_string = "camelCasingIsFun"

my_string.swapcase()

print(my_string)
print(my_string.swapcase())
```
