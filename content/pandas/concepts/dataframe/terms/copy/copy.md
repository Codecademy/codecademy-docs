---
Title: '.copy()'
Description: 'Returns a copy of a DataFrame or Series.'
Subjects:
  - 'Computer Science'
  - 'Data Science'
  - 'Web Development'
Tags:
  - 'Data Structures'
  - 'Pandas'
CatalogContent:
  - 'learn-python-3'
  - 'paths/data-science'
---

In Pandas, .copy() is a method that creates a copy of a DataFrame or a Series. This method either returns a fully independent copy of dataframe or a shallow copy (see Shallow vs. Deep Copy section).

## Syntax
```pseudo
df_copy = df.copy()
```

| Parameter Name | Data Type                | Usage                                                                                                                             |
| :------------: | ------------------------ | --------------------------------------------------------------------------------------------------------------------------------- |
|     `deep`     | bool                     | This argument specifies whether the copy should be a deep copy or a shallow copy. If deep=True, then the copy is a deep copy      |
|    `inplace`   | bool                     | If inplace=False (the default), the copy is made to a new object, and the original object is left unchanged.                      |
|     `meta`     | python dict              | This argument is used to specify metadata to be attached to the copy                                                              |

## Shallow vs. Deep Copy

Notice that .copy() method has a deep parameter that can dictate the behavior of the resulting dataframe. We can either make a shallow or a deep copy of pandas dataframe.
1. In a shallow copy, the new object points to the same data as the original object, and any changes made to the copy will affect the original object. Changes made to the original dataframe will also be reflected in the shallow copy. By default, .copy() creates a shallow copy. But you can set deep=False to enforce a shallow copy.

2. In a deep copy, a new object is created with a completely new set of data that is identical to the original data. Changes made to the copied object will not affect the original object and vice versa, even if the original data is modified. You can set deep=True to enforce a deep copy.

## Example:

```py
import pandas as pd

# create a DataFrame
df = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6]})

# create a deep copy of the DataFrame
deep_copy = df.copy(deep=True)

# create a shallow copy of the DataFrame
shallow_copy = df.copy(deep=False)

# modify the deep copy
deep_copy['A'][1] = 20

# modify the shallow copy
shallow_copy['A'][0] = 10

# print the deep copy
print(deep_copy)

# Output
#     A  B
# 0   1  4
# 1  20  5
# 2   3  6

# Changes are reflected in the deep copy.

# print the shallow copy
print(shallow_copy)

# Output
#     A  B
# 0  10  4
# 1   2  5
# 2   3  6

# Changes are reflected in the shallow copy

# print the original DataFrame
print(df)

# Output
#     A  B
# 0  10  4
# 1   2  5
# 2   3  6

# Changes made to the shallow copy, have also affected the original dataframe. But changes made
# to the deep copy have not affected the original dataframe.
```