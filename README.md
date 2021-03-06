# RangeSliderSwiftUI
Custom range slider in SwiftUI


[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg?style=flat)](https://github.com/Jigneshmayani90/RangeSliderSwiftUI/blob/main/LICENSE)
[![iOS](https://img.shields.io/badge/Platform-iOS-orange.svg?style=flat)](https://developer.apple.com/ios/)
[![Swift 5+](https://img.shields.io/badge/Swift-5+-orange.svg?style=flat)](https://developer.apple.com/swift/)
[![RangeSlider](https://img.shields.io/badge/Range-Slider-orange.svg?style=flat)](https://github.com/Jigneshmayani90/RangeSliderSwiftUI/)
[![SwiftUI](https://img.shields.io/badge/SwiftUI-orange.svg?style=flat)](https://developer.apple.com/swiftui/)
[![SPM](https://img.shields.io/badge/SPM-orange.svg?style=flat)](https://swift.org/package-manager/)

Custom range slider in SwiftUI

## Installation

#### SPM (Swift Package Manager)
In Xcode, use the menu File > Swift Packages > Add Package Dependency... and enter the package URL `https://github.com/Rahul-Mayani/RRRangeSliderSwiftUI`.

#### Manually
1. Download the project.
2. Add `RRRangeSliderSwiftUI.swift` file for slider view
3. Add necessary files in your project.
4. Congratulations!  

## Usage example
To run the example project, clone the repo, and run pod install from the Example directory first.

![alt text](https://github.com/Jigneshmayani90/RangeSliderSwiftUI/blob/main/sample.mp4)

```
@State var minValue: Float = 0.0
@State var maxValue: Float = Float(UIScreen.main.bounds.width - 50.0)

var body: some View {
    
    VStack {
        
        Text("Range Slider")
        /// slider view
        RRRangeSlider(
            minValue: self.$minValue, // mimimum value
            maxValue: self.$maxValue, // maximum value
            sliderWidth: CGFloat(maxValue), // set slider width
            backgroundTrackColor: Color(UIColor.systemTeal).opacity(0.5), // track color
            selectedTrackColor: Color.blue.opacity(25), // track color
            globeColor: Color.orange, // globe background color
            globeBackgroundColor: Color.black, // globe rounded border color
            globeMinMaxValuesColor: Color.black // all text label color
        )
    }
}


```

## Contribute 

We would love you for the contribution to **RangeSliderSwiftUI**, check the ``LICENSE`` file for more info.


## License

RangeSliderSwiftUI is available under the MIT license. See the LICENSE file for more info.
