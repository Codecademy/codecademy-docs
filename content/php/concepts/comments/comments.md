---
Title: "Comments"
Subjects:
  - "Web Development"
  - "Computer Science"
Tags: 
  - "Comments"
  - "Documentation"
CatalogContent:
  - "learn-php"
  - "paths/web-development"
  - "paths/computer-science"
---

Comments are text placed inside code that is not executed. They are intended as documentation or explanation of the code they are a part of.

## Syntax

PHP marks comments in three different ways:

- `//` will mark a comment from where it appears until the end of the line (or code block).
- `#` will also mark a comment from where it appears until the end of the line (or code block).
- Multi-line comments are marked by `/*` ... `*/` with everything in between marked as a comment.

Single line comments extend to the end of the line, or the end of the PHP block. 
`?>` will not be commented out, instead, `?>` will terminate the comment.

```php
<?php
  echo 'Testing 1, 2, 3...' // This is a single line comment

  /* This
     is
     a multi-line comment */

  echo 'Hello World!' # This is another single-line comment

// This comment ends with the enclosing block ?>
```

Note that attempting to nest multi-line comments will result in an error. The first comment ends when the first `*/` is encountered,
leaving the remaining comment(s) to be executed.

```php
<?php
  /* This is one multi-line comment
    /* But this inner comment will cause problems */
       This part of the comment will be executed
       since the end of the inner comment ended the outer
       comment as well. */
?>
```
