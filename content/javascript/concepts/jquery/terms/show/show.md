---
Title: '.shows()'
Description: 'Shows a hidden HTML element.'
Subjects:
  - 'Web Development'
  - 'Computer Science'
Tags:
  - 'DOM'
  - 'Events'
  - 'Functions'
  - 'jQuery'
  - 'Methods'
CatalogContent:
  - 'introduction-to-javascript'
  - 'paths/full-stack-engineer-career-path'
---

The **`.show()`** method shows a hidden [HTML element](https://www.codecademy.com/resources/docs/html/elements).

## Syntax

```pseudo
$(selector).show(speed, callback);
```

- `selector`: Specifies the elements that will be shown.
- `speed`(optional): Can be "slow" or "fast" or the number of milliseconds.
- `callback`(optional): A [function](https://www.codecademy.com/resources/docs/javascript/callbacks) that is called once showing is complete.

## Example

The following jQuery code will show the element selected with `#hide` when the `#show` element is clicked:

```js
$('#show').click(function () {
  $('#hide').show();
});
```
