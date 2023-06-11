---
Title: '.firstIndexOf()'
Description: 'Returns the index of the first element in an array that satisfies the given condition.'
Subjects:
  - 'Swift'
  - 'Mobile Development'
Tags:
  - 'Arrays'
  - 'Methods'
  - 'Searching'
CatalogContent:
  - 'learn-swift'
  - 'paths/build-ios-apps-with-swiftui'
---

The **`.firstIndexOf()`** method in Swift returns the index of the first element in an array that fulfills a specified condition. If no element satisfies the condition, it returns **`nil`**.

## Syntax

```pseudo
arrayName.firstIndexOf { condition }
```

The **`.firstIndexOf()`** method takes a single parameter, which is a closure representing the condition that an element must satisfy. The closure returns a boolean value indicating whether a particular element meets the condition.

## Example

Consider an array of integers representing the temperatures in Celsius:

```swift
let temperatures = [23, 18, 25, 20, 22, 21]
```

We can use the **`.firstIndexOf()`** method to find the index of the first temperature that exceeds a certain threshold, such as 25 degrees:

```swift
let threshold = 25

if let index = temperatures.firstIndexOf({ $0 > threshold }) {
    print("The first temperature exceeding \(threshold) degrees is at index \(index).")
} else {
    print("No temperature exceeds \(threshold) degrees.")
}
```

In this example, the closure **`{ $0 > threshold }`** is used as the condition. It checks whether each temperature in the array is greater than the threshold. If a temperature exceeding the threshold is found, the index of that temperature is printed. Otherwise, a message indicating that no temperature exceeds the threshold is printed.

The output will be:

```csharp
The first temperature exceeding 25 degrees is at index 2.
```

In this case, the temperature 25 is the first element in the array that satisfies the condition, and its index is 2.

Note that the .firstIndexOf() method returns an optional value, so we use optional binding (if let) to safely unwrap the result.

> **"Note: The `.firstIndexOf()` method is available in Swift 4.2 and later versions."**
