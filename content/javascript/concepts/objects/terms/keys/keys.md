---
Title: 'Object.keys()'
Description: 'Extracts keys from an object and returns them as an array'
Subjects:
  - 'Web Development'
  - 'Computer Science'  
Tags:
  - 'Objects'
  - 'Methods'  
CatalogContent: 
  - 'introduction-to-javascript'
  - 'paths/front-end-engineer-career-path'
---

The `Object.keys()` static method is used to extract keys from an object and returns them as an array. `Object.keys()` only returns the keys for the object's property
and only for enumerable properties.

>**Note:** The order of the keys in the resulting array is not guaranteed to be the same as the order in which they were defined in the object.

## Syntax

The basic syntax is:

```pseudo
Object.keys(obj)
```

- `obj` - An object.

## Example

Here's a simple example:
```js
const myObject = {
  name: 'John',
  age: 25,
  city: 'London'
};
const keysArray = Object.keys(myObject);
console.log(keysArray);
```
### Output:

```pseudo
  ['name', 'age', 'city']
```
