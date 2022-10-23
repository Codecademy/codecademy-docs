---
Title: '.subtractExact()'
Description: 'Returns the difference of two arguments.'
Subjects:
  - 'Computer Science'
Tags:
  - 'Arithmetic'
  - 'Functions'
  - 'Methods'
  - 'Numbers'
CatalogContent:
  - 'learn-java'
  - 'paths/computer-science'
---

The **`Math.subtractExact()`** method returns the difference of two arguments.

`Math.subtractExact()` accepts two arguments either of type `long` or `int`. If the value of any of the arguments exceeds its type's minimum or maximum value, then `ArithmeticError` is thrown (which is not the case with the subtraction operator), ensuring that the output is within the boundaries.

Also, using `Math.subtractExact()` helps ensure that the values being subtracted are integers and not floating point numbers.

## Syntax

```pseudo
Math.subtractExact(x, y)
```

The type of the value returned by `.subtractExact()` method depends upon the arguments passed:

- If both the arguments are of type `int`, then the return type will be `int`.
- If both the arguments are of type `long`, then the return type will be `long`.
- If one of the arguments is of `long`, type then the return will be `long`.

## Example

The following example demonstrates the `.subtractExact()` method:

```java
// Check.java
public class Check {
  public static void main(String args[]) {
    long x = 64L;
    long y = 49L;
    System.out.println(Math.subtractExact(x, y));
  }
}
```

This results in the following output:

```shell
15
```
