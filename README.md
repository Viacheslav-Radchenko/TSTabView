TSTabView
=======

`TSTabView` is a container component for set of views or view controllers.

<img src="https://raw.github.com/Viacheslav-Radchenko/TSTabView/master/Screenshots/TSTabView_Screenshot1.jpg" alt="TSTabView examples" width="360" height="480" />
<img src="https://raw.github.com/Viacheslav-Radchenko/TSTabView/master/Screenshots/TSTabView_Screenshot2.jpg" alt="TSTabView examples" width="360" height="480" />

## TSTabViewWithDropDownPanel

`TSTabViewWithDropDownPanel` extends `TSTabView`. Custom view can be attached to drop down panel which pull down/up on top of tabs container.

<img src="https://raw.github.com/Viacheslav-Radchenko/TSTabView/master/Screenshots/TSTabViewWithDropDownPanel_Screenshot1.jpg" alt="TSTabViewWithDropDownPanel examples" width="360" height="480" />

## Requirements

* Xcode 4.5 or higher
* Apple LLVM compiler
* iOS 5.0 or higher
* ARC
* QuartzCore.framework

## Demo

Build and run the `TSTabView ` project in Xcode to see examples of each component.
Right now better way to see components functionality is to compile examples provided with project, they fully display structure and dynamics of controls, as well as possible use cases.

## Installation

All you need to do is drop source files from `Classes\TSUIKit` folder into your project and add corresponding `#include "*.h"` to the top of classes that will use particular component.
`TS*Models` are optional part of `TSTabView` infrastructure. They provide ready-to-use examples of corresponding data source implementations. You may use them or implement your own data sources.
`TSTabView` use `QuartzCore.framework`, so you might need to add it as well.

## Contact

Viacheslav Radchenko

- https://github.com/Viacheslav-Radchenko
- radchencko.v.i@gmail.com

## License

TSTabView is available under the MIT license.

Copyright © 2013 Viacheslav Radchenko.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
