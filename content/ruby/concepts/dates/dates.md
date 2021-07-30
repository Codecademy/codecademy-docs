---
Title: "Dates"
Subjects:
  - "Web Development"
  - "Computer Science"
Tags: 
  - "Date"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-ruby"
  - "https://www.codecademy.com/learn/paths/web-development"
---

In Ruby, date- and time-specific data are handled by two classes: 

* `Date`
* `DateTime`

In order to use these classes, import the `date` module: 

```rb
require("date")
```

## Syntax

To create a new `Date` object, use `.new()`: 

```rb
# with 1 argument 
myDate = Date.new(year)

# with 2 arguments
myDate = Date.new(year, month)

# with 3 arguments 
myDate = Date.new(year, month, day)

myDate = Date.new(2021, 07, 30)

puts myDate # Output: 2021-07-30
```

To create a new `DateTime` object, use `.new()`:

```rb
require("date")

myDateTime = DateTime.new(year, month, day, hour, minute, second, offset)

myDateTime = DateTime.new(2021, 07, 30, 13, 46, 45, "+4")

puts myDateTime # Output: 2021-07-30T13:46:45+04:00
```

To create a new `DateTime` object set to this very moment, use `.now()`: 

```rb
puts DateTime.now # Output: 2021-07-30T13:48:56-04:00
```