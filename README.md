# iOS Sample Code

## Index
- <a href="https://github.com/theFlawlessHack/ios-sample-code/blob/master/README.md#rounded-button-edges">Rounded Button Edges</a>

## Rounded Button Edges
Rounding the edges of a button occurs by referencing the button's layer and making modifications to the button's corner radius. The button can be referenced using an IBOutlet. In the example the button name can be replaced with the name of your button's name.<br><br>

Typically, the button edge rounding will occur in the view did load function or in a function dedicated to making modifiications to the views.

```
import UIKit
@IBOutlet weak var buttonName: UIButton!

override func viewDidLoad() {
  super.viewDidLoad()
  
  // some arbitrary value for the curve
  buttonName.layer.cornerRadius = 15
  
  // a completely oval curved edge
  buttonName.layer.cornerRadius = buttonName.layer.frame.height / 2
}
```
