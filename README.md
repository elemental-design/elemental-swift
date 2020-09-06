# elemental-swift
Elemental Swift – build design systems for SwiftUI

## Initial Specification

### Components

- `<Box>` -> `HStack`
- `<Row>` -> `VStack`
- `<Pressable>` -> `Button`

### Pseudo-Code

```swift
struct Box: View {
  var body: some View {
    HStack()
  }
}

struct Pressable: View {
  var label: String

  var body: some View {
    Button(action: {
          self.isTimerActive.toggle()
      }, label: {
          Text(label)
              .frame(minWidth: 64)
      })
          .buttonStyle(PlainButtonStyle())
  }
}
```
