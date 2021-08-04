---
Title: "Attributes"
Subjects:
  - "Web Development"
  - "Web Design"
Tags:
  - "Attributes"
  - "Elements"
  - "Tags"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-html"
  - "https://www.codecademy.com/learn/paths/web-development"
---

HTML attributes consist of a name and a value using the following syntax: `name="value"`. They can be added to the opening tag of an HTML element to configure or change the element's default behavior and provide additional information about the element.

```html
<tag name="value"></tag>
```

So for example, the HTML `<img>` image element has a `src` attribute that contains the image URL and is mandatory:

```html
<img src="image.png">
```

## Unique ID Attributes

In HTML, specific and unique `id` attributes can be assigned to different elements in order to differentiate between them.

When needed, the `id` value can be called upon by CSS and JavaScript to manipulate, format, and perform specific instructions on that element and that element only. Valid id attributes should begin with a letter and should only contain letters (`a-Z`), digits (`0-9`), hyphens (`-`), underscores (`_`), and periods (`.`).

```html
<h1 id="A1">Hello World</h1>
```

## Example

In the provided example, we are giving the `<p>` paragraph element an unique identifier using the `id` attribute and changing the color of the default text using the `style` attribute:

```html
<p id="my-paragraph" style="color: green;">
  Here’s some text for a paragraph that is being altered by HTML attributes
</p>
```
