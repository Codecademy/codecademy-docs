---
Title: "Headings"
Subjects:
  - "Developer Tools"
  - "Web Development"
Tags: 
  - "Markdown"
  - "Headings"
  - "GitHub"
CatalogContent:
  - "paths/learn-how-to-build-websites"
  - "paths/web-development"
---

Headings are titles or subtitles that you want to display with markdown. There is a total of 6 different headings.

To create a heading, add hashtag signs `#` in front of a word or phrase. 

The number of number signs you use should correspond to the heading level. For example, to create a heading level three `<h3>`, use three number signs (e.g., `### My Header`).

## Syntax

```
# Heading level 1

## Heading level 2

### Heading level 3

#### Heading level 4

##### Heading level 5

###### Heading level 6
```

<h1>Heading level 1</h1>	

<h2>Heading level 2</h2>	

<h3>Heading level 3</h3>	

<h4>Heading level 4</h4>

<h5>Heading level 5</h5>

<h6>Heading level 6</h6>	

## Alternate Syntax

Alternatively, on the line below the text:

- Add any number of `==` characters for heading level 1 
- Add any number or `--` characters for heading level 2.

```
Heading level 1
===============	

Heading level 2
---------------	
```

## Best Practices

Markdown applications don’t agree on how to handle a missing space between the number signs (`#`) and the heading name. 

For compatibility, always put a space between the number signs and the heading name.

| ✅ Do | ❌ Don't |
| --- | --- |
| `# Here's a Heading` | `#Here's a Heading` |
  
<br>

You should also put blank lines before and after a heading for compatibility.

```
... text ends here.

# Heading

More text starts here.
```

## Example

```
# Headings

This page is about headings.

## The cool things about headings

Headings are great way to format the page.

## Example

Here's an example of headings.
```

