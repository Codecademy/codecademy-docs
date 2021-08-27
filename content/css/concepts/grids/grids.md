---
Title: "Grids"
Subjects:
  - "Web Development"
  - "Web Design"
Tags: 
  - "Grid"
  - "Elements"
  - "Properties"
CatalogContent:
  - "learn-css"
  - "paths/front-end-engineer-career-path"
---

CSS Grid is a two-dimensional grid-based layout system, with rows, columns and gaps. This layout system makes it easier to design and fine-tune the layout of web pages without having to use positioning and floats.

## Grid Elements

A grid layout consists of a parent element, with one or more child elements.

```html
<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>
  <div class="grid-item">4</div>
</div>
```

An HTML element becomes a grid container when its `display` property is set to `grid` or `inline-grid`:

```css
.grid-container {
  display: grid;
}
```

All the nested elements inside the grid container element are called _grid items_.

The difference between the values `inline-grid` and `grid` is that the `inline-grid` will make the element inline while `grid` will make it a block-level element.
 
- Grid columns are the verticle lines of the grid items.
- Grid rows are the horizontal lines of grid items.
- Grid gaps are the spaces between each column/row.

