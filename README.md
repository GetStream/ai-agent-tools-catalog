# Enter Swift
Learn fundamental Swift concepts with visual examples using SwiftUI. Contact Amos on Twitter: @amos_gyamfi. Each Swift concept explained and illustrated with tangible examples.

## What are Type Aliases?
```swift
import SwiftUI

/*
 Type aliases define an alternative name for an existing type. You define type aliases with the typealias keyword.
 Type aliases are useful when you want to refer to an existing type by a name that’s contextually more appropriate.
*/

struct TypeAliases: View {
    typealias Emoji = String
    let smiley: Emoji = "😊"
    let winkingFace: Emoji = "😉"
    let moneyFace: Emoji = "🤑"
    let 💞: Emoji = "Revolving Hearts"
    
    var body: some View {
        List {
            Text("Smiley face: \(smiley)")
            Text("Winking face: \(winkingFace)")
            Text("Money face: \(moneyFace)")
            Text(💞)
        }
    }
}

struct TypeAliases_Previews: PreviewProvider {
    static var previews: some View {
        TypeAliases()
            .preferredColorScheme(.dark)
    }
}
```
![Characters as constant and variable names](https://github.com/GetStream/enter-swift/blob/main/GifPreviews/typeAliases.png)

---

## How to name constants and variables with characters
Swift alows you to name variables and constants using characters, including Unicode. [CharacterConstantVariableNames.swift](https://gist.github.com/amosgyamfi/cf9fa33b4a5588788a2403429f3fa9d1#file-characterconstantvariablenames-swift)
![Characters as constant and variable names](https://github.com/GetStream/enter-swift/blob/main/GifPreviews/characterNames.png)



