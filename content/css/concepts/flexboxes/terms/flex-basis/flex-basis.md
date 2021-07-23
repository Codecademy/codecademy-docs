---
Title: "flex-basis"
Subjects:
  - "Web Development"
  - "Web Design"
Tags:
  - "Flexbox"
  - "Layout"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-css"
  - "https://www.codecademy.com/learn/paths/front-end-engineer-career-path"
  - "https://www.codecademy.com/learn/paths/full-stack-engineer-career-path"
---

## Definition

A property that defines the default size of a flex item.

## Syntax

```css
#item-a {
  display: flex;
  flex-basis: <flex-value>;
}
```

The `<flex-value>` can be any of the following:
- Grid keyword ( some are not well supported ) : `auto`, `max-content`, `min-content`
- Pixel value: `300px`
- Percent value: `25%`

## Example 1

An image that has a starting width of 200 pixels:

```css
#img-gallery {
  display: flex;
  flex-flow: row wrap; 
}

#img-one {
  display: flex;
  flex-basis: 200px; 
}
```
