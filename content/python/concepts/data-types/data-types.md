---
Title: 'Data Types'
Subjects:
  - 'Computer Science'
  - 'Data Science'
Tags:
  - 'Data Types'
  - 'Integers'
  - 'Booleans'
  - 'Strings'
CatalogContent:
  - 'learn-python-3'
  - 'paths/computer-science'
---

Python is a strongly typed language. Strongly typed means that the data type of a value doesn't change in unexpected ways.

```py
codecademy = 575
codecademy = "575 broadway"
```

After line 1, `codecademy` is an `int`. After line 2, `codecademy` is a `str`.

Here are Python's built-in data types:

- String type: `str`
- Boolean type: `bool`
- Binary types: `bytes`, `bytearray`, `memoryview`
- Number types: `int`, `float`, `complex`
- Sequence Types: `list`, `range`, `tuple`
- Set types: `set`, `frozenset`
- Dictionary type: `dict`

## type()

To find the data type of any object, the `type()` function can be used:

```py
message = "Hello, world!"

print(type(message))
```

This will output:

```shell
<class 'str'>
```

## isinstance()

You can also use the built-in `isinstance()` function to test if a variable is an instance of a specified type:

```py

word = "purple"
languages = ("Python", "JavaScript", "Go")

print(isinstance(word, str))
print(isinstance(languages, list))
print(isinstance(languages, tuple))
```

This will print a boolean value for each function call indicating if the object is an instance of the given type:

```shell
True
False
True
```
