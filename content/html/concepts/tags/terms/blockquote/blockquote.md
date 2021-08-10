---
Title: "<blockquote>"
Description: "Represents a section of a document which contains a longer quotation, usually spanning multiple lines."
Subjects:
  - "Web Development"
  - "Web Design"
Tags:
  - "Tags"
CatalogContent:
  - "learn-html"
  - "paths/web-development"
---

 

Represents a section of a document which contains a longer quotation, usually spanning multiple lines. 
  
A `<blockquote>` will often be shown by the browser indented from the surrounding text.

## Syntax

```html
<blockquote cite="citation url">
  <!-- The quotation goes inside the tag -->
</blockquote>
``` 

`<blockquote>` is a tag that wraps around a block of HTML. If there is a URL that the quotation comes from, the attribute `cite` may be used to indicate it. It behaves similar to a `<div>`, but will often have a left margin set by the browser by default.

## Example

Suppose that an article with a long and important quote is being written for a web page. The quote should be wrapped in `<blockquote>` as seen below:

```html
<html>
  <head>
  </head>
  <body>
    <article>
      <h2>Article Title</h2>
      <p>First paragraph of article.</p>
      <p>Second paragraph of article.</p>
      <blockquote>
        <p>Important quote that needs to stand out.<p>
        <p>Author Name, Quote Source</p>
      </blockquote>
      <p>Conclusion to article.</p>
    </article>
  </body>
</html>
```
