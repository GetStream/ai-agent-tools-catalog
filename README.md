# Animatable Swiftui Properties Index
A SwiftUI property is animatable if it can be changed to animate over time.  This repo serves developers all animatable SwiftUI properties with practical and real examples. Want to know how to animate a property not listed here? No problem. Contact Amos on Twitter: @amos_gyamfi

------------

## Alignment 
<p align="center">
 <img src="https://github.com/GetStream/animatable-swiftui-properties-index/blob/main/GifPreviews/alignmentProperty.gif"/>
</p>

```swift

 ZStack(alignment: movingAlignment ? .topTrailing : .bottomTrailing) {
                Image("userAmos")
                    .resizable()
                    .frame(width: 56, height: 56)
                    .clipShape(Circle())
                //User status: Online or offline
                Circle()
                    .frame(width: 12, height: 12)
                    .foregroundColor(onlineColor)
                    .animation(.default.delay(1).repeatForever(autoreverses: true), value: movingAlignment)
                    .onAppear{
                        movingAlignment.toggle()
                    }
            }
```
