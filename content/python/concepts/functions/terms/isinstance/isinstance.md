---
Title: 'isinstance()'
Description: 'Returns a boolean indicating if the given object is the specified type.'
Subjects:
  - 'Data Science'
  - 'Data Visualization'
  - 'Computer Science'
Tags:
  - 'AI'
  - 'Algorithms'
  - 'Booleans'
CatalogContent:
  - 'learn-python-3'
  - 'paths/computer-science'
---

The **isinstance()** function determines whether one object is a designated value type. If it is, the function will return `True`, otherwise the function will return `False`.

## Syntax

```pseudo
isinstance(object, type)
```

[Python Data Types](https://www.codecademy.com/resources/docs/python/data-types)

The example below demonstrates the use of the `isinstance()` function to test if multiple objects are of type `str`:

## Example

```py
var1 = "Hello World!"
var2 = 123

def check_if_string(value):
    if isinstance(value, str):
        print(f'{value} is a string type.')
    else:
        print(f'{value} is not a string.')

check_if_string(var1)
check_if_string(var2)
```

This example results in the following output:

```shell
Hello World! is a string type.
123 is not a string.
```
