---
Title: 'deg2rad()'
Description: 'Converts the number in degrees to the radian equivalent'
Subjects:
  - 'Computer Science
  - 'Web Development
  - 'Math Functions'
Tags:
  - 'Arithmetic'
  - 'Functions'
CatalogContent:
  - 'learn-php'
  - 'paths/computer-science'
---

The **`deg2rad()`** function converts the number in degrees to the radian equivalent.

The result returns a value type of `float`.

## Syntax

```pseudo
$result = deg2rad(n);
```

Where `n` is the number in degrees to be converted to the radian equivalent.

## Example

```php
echo deg2rad(90);
// Output: 1.5707963267949
```

The result will be a float value of `1.5707963267949` as the function converts degree `90` to the radian equivalent `1.5707963267949`.

## Codebyte Example

Using `deg2rad()` to convert degrees to radians`:

```codebyte/php
<?php
  echo deg2rad("360");
?>
```
