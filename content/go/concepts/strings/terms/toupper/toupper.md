---
Title: 'ToUpper()'
Description: 'Returns a string in all uppercase.'
Subjects:
  - 'Code Foundations'
  - 'Computer Science'
Tags:
  - 'Strings'
  - 'Functions'
CatalogContent:
  - 'learn-go'
  - 'paths/computer-science'
---

The **`ToUpper()`** function is used to convert lowercase alphabet to uppercase in a given string.

## Syntax

```pseudo
result = strings.ToUpper(str) 
```

The function accepts the given string, `str`, as its argument and returns the final string, `result`, converting lowercase characters to uppercase.

> **Note:** This only works with the standardized alphabet characters.

## Example

In the example below, the whole string "Codecademy" is converted to uppercase.

```go
package main
import (
   "fmt"
   "unicode"
)

func ToUpper(s string) string {
   a := []rune(s)
   for i, c := range a {
      if unicode.IsLower(c) {
         a[i] = unicode.ToUpper(c)
      }
   }
   return string(a)
}



func main() {
   var input string = "Codecademy"
   var output string = ToUpper(input)
   fmt.Println(output)
}
```

This example results in the following output:

```shell
CODECADEMY
```

## Codebyte Example

In the code below, a sentence in both lowercase and uppercase is converted into just uppercase using the `ToUpper()` function.

```codebyte/golang
package main
  
import (
    "fmt"
    "strings"
)
  
// Main method
func main() {
  
    str1 := "This is a Codecademy Tutorial"

    res1 := strings.ToUpper(str1)

    fmt.Println(res1)
```
