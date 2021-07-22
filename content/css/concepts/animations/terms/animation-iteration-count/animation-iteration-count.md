---
Title: "animation-iteration-count"
Subjects:
  - "Web Development"
  - "Web Design"
Tags:
  - "Animation"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-css"
  - "https://www.codecademy.com/learn/paths/front-end-engineer-career-path"
  - "https://www.codecademy.com/learn/paths/full-stack-engineer-career-path"
---

## Definition

Defines how many times an animation runs.

## Syntax

```css
animation-iteration-count: <value>;
```

where `<value>` can be one of the following:

- Number value: `3`, `300`
- `inifinite` will run animation on endless loop

**Note:** providing one value will apply to all `animation-name` values. Additional comma separated values will apply correspondingly.

## Example 1

Run animation `fadeoutfadein` two times:

```css
div {
  height: 200px;
  width: 200px;
  background-color: blue;
  animation-duration: 2s;
  animation-name: fadeoutfadein;
  animation-iteration-count: 2;
}

@keyframes fadeoutfadein {
  0% {
    background-color: blue;
  }
  50% {
    background-color: white;
  }
  100% {
    background-color: blue;
  }
}
```

## Example 2

Run animation `fadeoutfadein` two times and `slideleft` one time:

```css
div {
  height: 200px;
  width: 200px;
  background-color: blue;
  animation-duration: 4s, 4000ms;
  animation-name: fadeoutfadein, slideleft;
  animation-iteration-count: 1, 2;
}

@keyframes fadeoutfadein {
  0% {
    background-color: blue;
  }
  50% {
    background-color: white;
  }
  100% {
    background-color: blue;
  }
}

@keyframes slideleft {
  from {
    margin-left: 100%;
  }

  to {
    margin-left: 0%;
  }
}
```
