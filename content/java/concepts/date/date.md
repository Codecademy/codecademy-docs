---
Title: 'Date'
Description: 'The Date class in the java.util package is used to represent dates and times in Java'
Subjects:
  - 'Computer Science'
Tags:
  - 'Classes'
  - 'Date'
  - 'Methods'
CatalogContent:
  - 'learn-java'
  - 'paths/computer-science'
---

In simple terms, the `Date` [class](https://www.codecademy.com/learn/learn-java-classes-and-methods) represents a specific point in time, down to milliseconds. It provides methods to manipulate and format dates, as well as perform operations such as comparison and arithmetic. It internally stores the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 GMT (also known as the Unix epoch).

## Syntax

```pseudo
import java.util.Date;

public class DateExample {
    public static void main(String[] args) {

    Date currentDate = new Date();

    long currentTimeMillis = currentDate.getTime();

    System.out.println("Current date and time: " + currentDate);
    System.out.println("Milliseconds since Unix epoch: " + currentTimeMillis);
}
}
```

The output for the above code will be:

```shell
Current date and time: Wed Jun 16 12:34:56 GMT 2023
Milliseconds since Unix epoch: 1678450496000
```

In the above code, the `Date` class is imported from the `java.util` package. Inside the main method, a `Date` object named `currentDate` is created using the default constructor. This represents the current date and time. The number of milliseconds since the Unix epoch can be accessed using the `getTime()` method of the `Date` class. In the example, the value is assigned to the variable `currentTimeMillis`. Finally, the current date and time are displayed by printing the `currentDate` object using `System.out.println()`, and the number of milliseconds since the Unix epoch is also printed.

## Methods

Here are some important aspects and methods of the `Date` class:

- Creating a `Date` object:
  - `Date()`: Creates a Date object representing the current date and time.
  - `Date(long millis)`: Creates a `Date` object with the specified number of milliseconds since January 1, 1970, 00:00:00 GMT (the Unix epoch).
- Getting and setting date components:
  - `getTime()`: Returns the number of milliseconds since the Unix epoch.
  - `setTime(long time)`: Sets the time value of the Date object using the specified number of milliseconds.
- Formatting and parsing dates:
  - `toString()`: Returns a string representation of the Date object. The default format is not very readable or localized.
  - `SimpleDateFormat` class (from java.text package): Allows formatting and parsing of dates using patterns.
- Comparing dates:
  - `before`(Date when): Checks if the Date object is before the specified date.
  - `after`(Date when): Checks if the Date object is after the specified date.
  - `compareTo`(Date anotherDate): Compares the Date object with another Date object.
