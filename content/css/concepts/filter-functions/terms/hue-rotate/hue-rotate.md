---
Title: "hue-rotate"
Subjects:
  - "Web Development"
  - "Web Design"
Tags:
  - "Images"
  - "Functions"
  - "Colors"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-css"
  - "https://www.codecademy.com/learn/paths/front-end-engineer-career-path"
  - "https://www.codecademy.com/learn/paths/full-stack-engineer-career-path"
---

## Definition

CSS filter function accepts an angle value and rotates the hue of an element.

## Syntax

```css
filter: hue-rotate(<angle>);
```

where a required `<angle>` can be one of the following: `.25turn`, `-45deg`, `1.57rad`, `31.3grad` 

**Note:** Positive values increase the hue, negative values decrease the hue. A default value of `0` results in no change.

## Example 1

Rotate the hue of the image by 45 degrees:

```css
.banner-image {
    filter: hue-rotate(45deg);
}
```

