---
Title: 'freeze()'
Description: 'Make table read-only.'
Subjects:
  - 'Computer Science'
  - 'Game Development' 
Tags:
  - 'Tables'
  - 'Functions'
CatalogContent:
  - 'learn-lua'

---

Lua **`freeze()`** function freezes the provided table, and makes it read-only.

## Syntax

```lua
table.freeze(f)
```

The `freeze()` function attempts to freeze a specified non-frozen table named `f`. The function will fail if `f` is not a table or is already frozen.The function will
 Return the expected table `f`.
 This function helps to easily identify immutable functions for correctness purpose.

## Example

To freeze food in your fridge:

```lua
local frozen_table = table.freeze({
    "🍎",
    "🍌",
    "🍇",
    "🍓",
    "🍉"
})
```
We intiate a table `frozen_table` , then use the `freeze()` to freeze the table contents.
Now if you run:
```lua
frozen_table[1] = "🍔" -- This will throw an error
```
The error is caused because because the `freeze()` method has made the table `read-only` and we cannot modify its contents.


