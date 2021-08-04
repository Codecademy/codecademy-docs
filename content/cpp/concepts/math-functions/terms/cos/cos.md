---
Title: "cos()"
Description: "Returns the cosine of an argument given in radians."
Subjects:
  - "Computer Science"
Tags:
  - "Functions"
  - "Arithmetic"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-c-plus-plus"
  - "https://www.codecademy.com/learn/paths/computer-science"
---

## Definition

Returns the cosine of an argument given in radians.

## Syntax

```cpp
std::cos(n)
```

## Example 1

Use `cos()` to return the cosine of `3.1416` radians:

```cpp
#include <iostream>
#include <cmath>

int main() {
  double x = 3.1416;
  double result;

  result = std::cos(x);

  std::cout << "The cosine of " << x << " radians is " << result << "\n";
  // Output: The cosine of 3.1416 radians is -1
}
```
