---
Title: ".seed()"
Subjects:
  - "Computer Science"
  - "Data Science"
Tags:
  - "Random"
  - "Methods"
  - "Functions"
  - "Strings"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-python-3"
  - "https://www.codecademy.com/learn/paths/computer-science"
  - "https://www.codecademy.com/learn/paths/data-science"
---

## Definition

Save the state of the pseudo-random number generator. Pseudo-random number generators appear to produce random numbers by performing some operation on a value. This value is the seed, which acts as the first "previous" value in the sequence of numbers. By using a particular seed value, a user is able to reproduce the same random numbers multiple times. If no value is input into the method, the random number generator will use the current system time to create the seed.

## Syntax

```py
random.seed()
```

## Example 1

Use `.seed()` to initialize the pseudo-random number generator in Python with the current-time value:

```codebyte/python
import random

random.seed()
print(random.random())
```

## Example 2


Use `.seed()` to initialize the pseudo-random number generator in Python with a particular value:

```codebyte/python
import random

random.seed(5)
print(random.random())
```

## Example 3

Use `.seed()` to initialize the pseudo-random number generator in Python with a particular value:

```codebyte/python
import random

random.seed(5)
print(random.random())
```
