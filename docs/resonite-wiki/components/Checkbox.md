# Component:Checkbox

> Source: https://wiki.resonite.com/Component:Checkbox

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Checkbox&diff=95800) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b3/CheckboxComponent.png/510px-CheckboxComponent.png)](https://wiki.resonite.com/File:CheckboxComponent.png) **Checkbox** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Checkbox** component is a [UIX](https://wiki.resonite.com/UIX "UIX") element used with a [Button](https://wiki.resonite.com/Button_(Component) "Button (Component)") component to provide a toggling state whenever the button is pressed.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `State` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The current state of thie check box. |
| `TargetState` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | The Bool field to drive with the state of the checkbox. |
| `CheckVisual` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The Bool field controlling visibility of the visual to display when the checkbox is in the checked state. |

Fields
Collapse

## Usage

Checkboxes are great for settings and options in your designs.

## Examples

[![A checkbox from the Resonite Essentials folder.](https://wiki.resonite.com/images/1/19/UIX_Checkbox_Example_01.png)](https://wiki.resonite.com/File:UIX_Checkbox_Example_01.png) A checkbox from the Resonite Essentials folder.

There is a checkbox UI Preset from the [Resonite Essentials](https://wiki.resonite.com/Resonite_Essentials "Resonite Essentials") folder that users can use as a starting point for checkboxes.

Typically you'd have a child of the checkbox's slot containing an [Image](https://wiki.resonite.com/Image_(Component) "Image (Component)") component, and that slot's Active property is driven using the CheckVisual property of the checkbox. In addition, you can have a [SpriteProvider](https://wiki.resonite.com/SpriteProvider_(Component) "SpriteProvider (Component)") driving the Image component.

Here is [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial on checkboxes:

![](https://i.ytimg.com/vi/B2G708bnBeM/hqdefault.jpg)

[OLD: Neos VR Tutorial: UIX Pt.6 - Checkboxes](https://www.youtube-nocookie.com/embed/B2G708bnBeM?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Checkbox&oldid=95800](https://wiki.resonite.com/index.php?title=Component:Checkbox&oldid=95800)"

Contents