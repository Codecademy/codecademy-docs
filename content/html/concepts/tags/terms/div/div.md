---
Title: "<div>"
Description: "The <div> tag represents a generic division of content. It has no semantic meaning, but will separate its contents from the rest of the document."
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

The `<div>` tag represents a generic division of content. It has no semantic meaning, but will separate its contents from the rest of the document.

## Syntax

```html
<div>
  <!-- Content lives here -->
</div>
``` 

`<div>` is a tag that wraps around a block of HTML. By default it is a block element, meaning its contents will start on a new line and the content that follows will start on a new line.

## Example

A `<div>` is a good choice when no other tag matches the content type. Additionally it is often used to help style an entire page, or sections of a page via the `class` or `id` attribute.

```html
<html>
  <head>
  </head>
  <body>
    <!-- This div wraps the entire site applying the styles from the dark-mode class -->
    <div class="dark-mode">
      <!-- Site content lives here -->
    </div>
  </body>
</html>
```