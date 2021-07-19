---
Title: "background-blend-mode"
Subjects:
  - "Web Development"
  - "Web Design"
Tags:
  - "Background"
  - "Colors"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-css"
  - "https://www.codecademy.com/learn/paths/front-end-engineer-career-path"
  - "https://www.codecademy.com/learn/paths/full-stack-engineer-career-path"
---

## Definition

Returns a new blended color based on the background color and the background images.

## Syntax

```css
background-blend-mode: <value>;
```

where `<value>` can be one of the following: `normal` | `multiply` | `screen` | `overlay` | `darken` | `lighten` | `color-dodge` | `color-burn` | `hard-light` | `soft-light` | `difference` | `exclusion` | `hue` | `saturation` | `color` | `luminosity`

- `normal` is the default value which imposes simple alpha blending, as CSS has permitted since its inception.

- `lighten` means that the final result will show, at each pixel, either the image or its backdrop, whichever is lighter.

- `darken` will show, at each pixel, whichever is darker.

## Example 1

The background color will not bleed through the background image:

```css
body {
  background-image: url("fish.jpg");
  background-color: blue;
  background-blend-mode: normal;
}
```

## Example 2

At each pixel, show whichever is lighter between the background image and the background color:

```css
body {
  background-image: url("fish.jpg");
  background-color: blue;
  background-blend-mode: lighten;
}
```

## Example 3

At each pixel, show whichever is darker between the background image and the background color:

```css
body {
  background-image: url("fish.jpg");
  background-color: blue;
  background-blend-mode: darken;
}
```
