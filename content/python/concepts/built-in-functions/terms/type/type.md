---
Title: 'type()'
Description: 'Returns the data type of an object.'
Subjects:
  - 'Computer Science'
  - 'Data Science'
Tags:
  - 'Built-in Functions'
  - 'Methods'
CatalogContent:
  - 'learn-python-3'
  - 'paths/computer-science'
---

A function that returns the data type of an object.

## Syntax

```pseudo
type(some_object)
```

The `type()` function primarily accepts `some_object` as a parameter, which can be any of Python's [data types](https://www.codecademy.com/resources/docs/python/data-types).

## Example

The `type()` function can be used to confirm the data type of the object `spam`:

```py
spam = 10

print(type(spam))

# Output: int
```

## Codebyte Example

The following example uses the `type()` function to return the data type of the `strings` object:

```codebyte/python
strings = ['foo', 'bar']

print(type(strings))
```
