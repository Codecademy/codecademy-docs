---
Title: '.attr()'
Description: 'Used to get or set attributes of selected elements.'
Subjects:
  - 'Data Visualization'
  - 'Computer Science'
Tags:
  - 'D3'
  - 'Style'
CatalogContent:
  - 'learn-d3'
  - 'paths/computer-science'
---

The **`.attr()`** method is used to set or get attributes of selected elements. This method is commonly used for styling elements by setting their attributes.

## Syntax

```pseudo
selection.attr("attributeName", "attributeValue");
```

The `.attr()` function takes two parameters,

- `attributeName`: Name of the attribute
- `attributeValue`: Value of the attribute or a callback function.

## Example

In the example given below, the value `5` is set to the attribute `radius` which turns the radius of `circle` to 5 units.

```js
d3.select('circle').attr('radius', 5);
```

The example given below demonstrates the argument as a callback function. It is used to dynamically compute attribute value based on the data given. Here the function is used to calculate the parameter of the circle. The callback function is passed the current data and returns the attribute value.

```js
d3.select('circle').attr('parameter', function (d) {
  return 2 * 3.14 * d.radius;
});
```
