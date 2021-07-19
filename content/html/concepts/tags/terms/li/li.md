---
Title: "<li>"
Subjects:
  - "Web Development"
  - "Web Design"
Tags:
  - "Tags"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-html"
  - "https://www.codecademy.com/learn/paths/web-development"
---

## Definition 

Represents a single item in a list of items. It and the other list items must be wrapped in an `<ol>`, `<ul>`, or `<menu>` tag.

## Syntax

```html
<li>Text for list item</li>
``` 

`<li>` is a tag that requires content between it and its closing tag. It can contain any valid HTML, and each `<li>` tag will be indented and preceded either with a number (for ordered lists), or a dot (for unordered lists and menus).

## Example

```html
<html>
  <head>
  </head>
  <body>
    <h3>My Favorite Things</h3>
    <ol>
      <li>Rain drops on roses</li>
      <li>Whiskers on kittens</li>
      <li>Bright copper kettles</li>
      <li>Warm woolen mittens</li>
    </ol>
  </body>
</html>
```
  
The `<ol>` creates an ordered list. The content from each `<li>` tag will have a number before it:

 1. Rain drops on roses
 2. Whiskers on kittens
 3. Bright copper kettles
 4. Warm wollen mittens
