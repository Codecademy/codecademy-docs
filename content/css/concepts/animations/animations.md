---
Title: 'Animations'
Description: 'A CSS animation lets an HTML element gradually change from one style to another without using JavaScript. To use CSS animation, some keyframes for the animation must be specified. Keyframes hold what CSS styles the element will have at certain times.'
Subjects:
  - 'Web Development'
  - 'Web Design'
Tags:
  - 'Animation'
  - 'Elements'
CatalogContent:
  - 'learn-css'
  - 'paths/front-end-engineer-career-path'
---

A CSS animation lets an HTML element gradually change from one style to another, without using JavaScript. Any number of CSS properties can be changed, for any amount of times.

To use CSS animation, some keyframes for the animation must be specified.

## `@keyframes` Rule

Keyframes hold what CSS styles the element will have at certain times. When specifying styles inside the `@keyframes` rule, the animation will gradually change from the current styles to the new styles.

To get an animation to work, the animation must be bound to an element and the `animation-duration` should be defined. In this example code, the `<h1>` element will load as yellow and gradually change to orange over the course of 5 seconds.

```css
/* The animation */
@keyframes color-change {
  from {
    color: yellow;
  }
  to {
    color: orange;
  }
}

/* The element */
h1 {
  color: yellow;
  animation-name: color-change;
  animation-duration: 5s;
}
```
