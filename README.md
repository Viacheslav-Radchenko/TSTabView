TSTabView
=======

`TSTabView` UI component that allows to flip left and right through pages of data. Pages content provided to TSTabView by implementing TSTabViewDataSource protocol. TSTabView can manage set of UIView or UIViewController objects. TSNavigationStripView control is used to display available pages titles/tabs and navigate between them.
Custom TSNavigationStripView entity should be provided to TSTabView during initialisation. Some features are listed below:

* Navigates through set of UIView or UIViewController objects.
* Support far jumps between pages.
* Tabs list in TSNavigationStripView support different types of layout and alignment, including: alignment to left side, alignment to right side, autofill available space, central alignment (which imitate behaviour of ViewPager component on Android).
* Tabs list in TSNavigationStripView can be scrollable.
* TSNavigationStripView can display additional menu items on left or right sides.
* TSNavigationStripView provide great flexibility for appearance  customisation.
* All view transitions are done with smooth animations.

<img src="https://raw.github.com/Viacheslav-Radchenko/TSUIKit/master/Screenshots/TSTabView_Screenshot1.jpg" alt="TSTabView examples" width="360" height="480" />
<img src="https://raw.github.com/Viacheslav-Radchenko/SSUIKit/master/Screenshots/TSTabView_Screenshot2.jpg" alt="TSTabView examples" width="360" height="480" />

Example of TSTabView object instantiation provided below.
```
TSNavigationStripView *navigationStripView = [[TSNavigationStripView alloc] initWithFrame:CGRectMake(0, 0, self.view.bounds.size.width, 32)];
// Customize navigation view appearance...

TSTabView *tabView = [[TSTabView alloc] initWithFrame:self.view.bounds navigationMenu:navigationStripView];
tabView.delegate = self;
[self.view addSubview: tabView];

TSTabViewModel *tabViewModel = [[TSTabViewModel alloc] initWithTabView:tabView];
[tabViewModel setTabs:@[
	[[TSTabViewSection alloc] initWithTitle:@"Tab 1" andView: /* Provide view */],
	[[TSTabViewSection alloc] initWithTitle:@"Tab 2" andView: /* Provide view */]]
];
```

## TSNavigationStripView

`TSNavigationStripView` is a navigation menu control with highly customizable design and flexible structure.
It provides smooth animations for item selection and dynamic content modification. Some features are listed below:

* Display set of section titles (tabs).
* Select section (tab) from list.
* Scroll between sections (tabs).
* Left and right navigation buttons on sides.
* Fully customized appearance (see examples).
* Support different types of layout and alignment: alignment to left side, alignment to right side, autofill available space, central alignment (which imitate behaviour of ViewPager component on Android).
* Additinal not scrolled menu items can be added on left and right sides.
            
<img src="https://raw.github.com/Viacheslav-Radchenko/TSUIKit/master/Screenshots/TSNavigationStripView_Screenshot1.jpg" alt="TSNavigationStripView examples" width="360" height="480" />

## TSTabViewWithDropDownPanel

`TSTabViewWithDropDownPanel` extends `TSTabView`. Custom view can be attached to drop down panel which pull down/up on top of tabs container.

<img src="https://raw.github.com/Viacheslav-Radchenko/TSTabView/master/Screenshots/TSTabViewWithDropDownPanel_Screenshot1.jpg" alt="TSTabViewWithDropDownPanel examples" width="360" height="480" />

## Links

* Parent repository [TSUIKit](https://github.com/Viacheslav-Radchenko/TSUIKit).
* Demo video [TSTabView](http://youtu.be/GvTfKJM43uQ).

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

The easiest way to integrate TSUIKit is using CocoaPods. Just add this to your Podfile:
```
	pod 'TSUIKit', '~> 0.1' 
```

Other option is to  drop source files from `Classes\TSUIKit` folder into your project and add corresponding `#include "*.h"` to the top of classes that will use particular component.
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
