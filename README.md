# DropDownAlert
Drop down alert for iOS

## Usage

#### Top
    let alert = DropDownAlert()
    alert.alertWith("U can use just title")
    
    alert.didTapBlock = {
      print("Top View Did Tapped")
    }
    
    let alert = DropDownAlert()
    alert.alertWith(titleString, message: messageString)
    
    alert.didTapBlock = {
      print("Top View Did Tapped")
    }
    
### Top With Directions
```swift
    let alert = DropDownAlert(position: .top, direction: .toLeft)
    alert.alertWith(titleString, message: messageString)
    
    alert.didTapBlock = {
      print("Top View Did Tapped")
    }
    
    let alert = DropDownAlert(position: .top, direction: .toRight)
    alert.alertWith(titleString, message: messageString, topLabelColor: UIColor.white, messageLabelColor: UIColor.darkGray, backgroundColor: UIColor.brown)

//  alert.alertWith(titleString, message: messageString, topLabelColor: UIColor.white, messageLabelColor: UIColor.darkGray)
//  alert.alertWith(titleString, message: messageString, topLabelColor: UIColor.white)
//  alert.alertWith(titleString, message: messageString)

    
    alert.didTapBlock = {
      print("Top View Did Tapped")
    }
```
### Bottom
```swift
    let alert = DropDownAlert(position: .bottom)
    alert.alertWith(titleString, message: messageString)
    
    alert.didTapBlock = {
      print("Bottom Alert View Did Tapped")
    }
```   
### Bottom With Directions
```swift
    let alert = DropDownAlert(position: .bottom, direction: .toLeft)
    alert.alertWith(titleString, message: messageString)
    
    alert.didTapBlock = {
      print("Bottom Alert View Did Tapped")
    }
    
    let alert = DropDownAlert(position: .bottom, direction: .toRight)
    alert.alertWith(titleString, message: messageString)
    
    alert.didTapBlock = {
      print("Bottom Alert View Did Tapped")
    }
```    
### Different Positions and Animation Directions
```swift
  enum AlertPosition {
    case top
    case bottom
  }
  
  enum AnimationDirection {
    case toLeft
    case toRight
    case normal
  }
 ``` 
### Requirements
iOS 8.0 +
Swift 3.0 +
Xcode 8.0 +
