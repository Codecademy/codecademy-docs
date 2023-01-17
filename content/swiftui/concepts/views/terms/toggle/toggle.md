---
Title: 'Toggle'
Description: 'Chooses between an "on or off" state based on a Bool type value.'
Subjects:
  - 'Mobile Development'
  - 'Computer Science'
Tags:
  - 'SwiftUI'
  - 'SwiftUI Views'
  - 'Toggle'
  - 'Views'
CatalogContent:
  - 'learn-swiftui'
  - 'paths/build-ios-apps-with-swiftui'
---

A **`Toggle`** is a View that chooses between "on or off" options based on a `Bool` type value.

## Syntax

```pseudo
Toggle("Title String", isOn: Binding<Bool>)
```

The following parameters can be applied to a `Toggle` view:

- The `"Title String"` parameter is used instead of a [closure](https://www.codecademy.com/resources/docs/swift/closures).
- `isOn:` is a binding `Bool` type parameter that determines the state of the toggle (on or off).

## Example

The following example displays a `Toggle` that turns a "Wi-Fi" switch on and off by passing the `isWifiOn` variable to the `isOn:` property. The `Label` will be inside a trailing closure.

```swift
@State var isWifiOn = false

var body: some View {
    Toggle(isOn: $isWifiOn) {
        Text("Wi-Fi")
    }
    .padding()
}
```

The `.padding()` view modifier adds some space to the attached the view. In this way, the toggle and its label are not squished to the end of the screen.

This will display the following when the `Toggle` is off:

![Toggle when off](https://raw.githubusercontent.com/Codecademy/docs/main/media/swiftui-toggle-off.png)

This will display the following when the `Toggle` is on:

![Toggle when on](https://raw.githubusercontent.com/Codecademy/docs/main/media/swiftui-toggle-on.png)
