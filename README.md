KYCDraggableVC
==============
Features
---

* works like UISplitViewController in iPhone/iPad
* Customizable properties:
  * KYC_Hide_LeftVC_Portion_In_ParentVC_Pos_X
  * KYC_Show_LeftVC_Portion_In_ParentVC_Pos_X
  * KYC_Set_LeftVC__Pos_Y
  * KYC_LeftVC_Closed_Pos_X
  * KYC_LeftVC_Open_Pos_X
  * KYC_Open_Close_LeftVC_Velocity
* Wholesome springy animation


Which files are needed?
---

* KYCDraggableViewController (.h .m)


How to use it
---

It’s very simple. Create your Left ViewController (.h .m) files with Storyboard/nib
Make KYCDraggableViewController as your Left ViewController's parent (e.g. to see the example project)
For Storyboard Id: set this 'LeftVCStoryboard' (You can change this)
The examples below demonstrate how to customize the appearance and value displayed.

```objective-c
    // (Optional) you can need to do this in Left ViewController in ViewDidLoad method.
    // set your LEFTVC settings here as per iPhone OR iPad
    self.KYC_Hide_LeftVC_Portion_In_ParentVC_Pos_X = -(self.view.frame.size.width - 20);
    self.KYC_Show_LeftVC_Portion_In_ParentVC_Pos_X = -1;
    self.KYC_Set_LeftVC__Pos_Y = 0;
    self.KYC_LeftVC_Closed_Pos_X = (self.view.frame.size.width - 20);
    self.KYC_LeftVC_Open_Pos_X = (self.view.frame.size.width - 20) - 1;
    self.KYC_Open_Close_LeftVC_Velocity = 750;
```
