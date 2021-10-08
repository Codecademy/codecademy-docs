---
Title: '.isInteger()'
Description: 'Determine whether the passed value is an integer.'
Subjects:
  - 'Web Development'
  - 'Computer Science'
Tags:
  - 'Numbers'
  - 'Methods'
CatalogContent:
  - 'introduction-to-javascript'
  - 'paths/front-end-engineer-career-path'
---

The `.isInteger()` method is a part of the `Number` class in JavaScript. It accepts a single argument, `value`, returns `true` if the passed argument is an integer, and returns `false` otherwise.

## Syntax

```js
Number.isInteger(value);
```

## Example

To verify if a value is an integer or not:

```js
const x = 13 / 5;
// x = 2.6

const y = 10 / 5;
// y = 2

console.log(Number.isInteger(x));
// Output: false

console.log(Number.isInteger(y));
// Output: true
```

The above example passes an integer and a decimal value into `Number.isInteger()` method, to verify if the value is an integer or not. Then, the result is printed.
