---
Title: "Loops in Java"
Subjects:
  - "Computer Science"
Tags: 
  - "Loops"
  - "While"
  - "For"
Catalog Content:
  - "https://www.codecademy.com/learn/learn-java"
  - "https://www.codecademy.com/learn/paths/computer-science"
---

## While Loop

The `while` loop loops through a block of code as long as a specified condition is true:

```pseudo
while (condition) {
  // Code block to be executed
}
```

In the example below, the code in the loop will run, over and over again, as long as a variable (i) is less than 5:

```java
int i = 0;

while (i < 5) {
  System.out.println(i);
  i++;
}
```

The output would be:

```
0
1
2
3
4
```

## For-Each Statement

In Java, the `for`-`each` statement allows you to directly loop through each item in an array or `ArrayList` and perform some action with each item.

When creating a `for`-`each` statement, you must include the `for` keyword and two expressions inside of parentheses, separated by a colon. These include:

- The handle for an element we’re currently iterating over.
- The source array or ArrayList we’re iterating over.

```java
// Array of numbers
int[] numbers = {1, 2, 3, 4, 5};
 
// For-each loop that prints each number in numbers
// int num is the handle while numbers is the source array
for (int num : numbers) {  
    System.out.println(num);
}
```
