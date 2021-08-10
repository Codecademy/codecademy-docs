---
Title: "<canvas>"
Description: "Creates an element in the page for JavaScript and WebGL to interact with, primarily to create and animate graphics within the page."
Subjects:
  - "Web Development"
  - "Web Design"
Tags:
  - "Tags"
CatalogContent:
  - "learn-html"
  - "paths/web-development"
---

 

Creates an element in the page for JavaScript and WebGL to interact with, primarily to create and animate graphics within the page.

## Syntax

```html
<canvas>
  Alternate text goes here, should the browser not support the canvas tag.
</canvas>
``` 

There are two major attributes associated with the `<canvas>` element, `height` and `width`. These will set the element height and width, in pixels. They default to a height of 150px, and a width of 300px.

## Example

Suppose that a multi-user whiteboard application needs a canvas for the users to interact with. Further, it is important that the canvas is 800px wide, and 600px tall. Additionally it is important to provide a fallback message should the canvas not work.

```html
<html>
  <head>
  </head>
  <body>
    <canvas width="800" height="600">
      <h3>Your browser does not support this feature. Please switch to another browser, if possible.</h3>
    </canvas>
  </body>
</html>
```
