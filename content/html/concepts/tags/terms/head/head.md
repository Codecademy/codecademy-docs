---
Title: "<head>"
Description: "The <head> tag represents a collection of metadata related to the current document. It is an immediate child of the <html> elemend and may include other tags such as <title>, <link>, <style>, and <script>."
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

The `<head>` tag represents a collection of metadata related to the current document. It is an immediate child of the `<html>` elemend and may include other tags such as `<title>`, `<link>`, `<style>`, and `<script>`.

## Syntax

```html
<head>
  <!-- Document-level metadata tags go here -->
</head>
``` 

`<head>` is a tag whose content does not get shown to the user, so there is no default formatting behavior. 

## Example

Suppose that the site needs a title shown in the browser, either in the tab or in the browser window. Additionally it needs to load some CSS rules to style the document, and a JavaScript script to allow some interactivity. 
  
The `<head>` tag is the perfect place to tell the document where these things live, and what they should be:

```html
<html>
  <head>
    <!-- This sets the title in the browser -->
    <title>My Home | Codecademy</title>

    <!-- This loads a stylesheet file called styles.css, and applies the rules to tags in the body -->
    <link rel="stylesheet" href="styles.css">

    <!-- This loads and executes a script from a file called app.js -->
    <script type="text/javascript" src="app.js"></script>
  </head>
  <body>
    <!-- User-facing content goes here -->
  </body>
</html>
```
