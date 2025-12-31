# Component:ButtonEditColorX

> Source: https://wiki.resonite.com/Component:ButtonEditColorX

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2a/ButtonEditColorXComponent.png/510px-ButtonEditColorXComponent.png)](https://wiki.resonite.com/File:ButtonEditColorXComponent.png) **Button Edit Color X** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonEditColorX** component takes in a [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") field, and when a button interacts with it, a [ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface") is created for the [user](https://wiki.resonite.com/User "User") (if the user has [Builder](https://wiki.resonite.com/Permission_System "Permission System")).

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

If the user does not have Builder and this component is under the button being pressed, it removes the button.


| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The target [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"). |
| `_colorPicker` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface") >** | The [ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface") component. |
| `Continuous` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes the color editing change continuous. |
| `Alpha` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allows for use of the alpha channel. |
| `HDR` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allows the use for HDR in this color. |

Fields
Collapse

## Usage

This is used to edit colors with a press of a button.

## Examples

### Videos

[ProbablePrime's](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime") Video on **ButtonEditColorX**.

![](https://i.ytimg.com/vi/RYJaQ6cCZzc/hqdefault.jpg)

[Resonite Tutorial: Button Edit ColorX](https://www.youtube-nocookie.com/embed/RYJaQ6cCZzc?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- Inspectors use a different component for changing colors using [ColorXMemberEditor](https://wiki.resonite.com/Component:ColorXMemberEditor "Component:ColorXMemberEditor").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonEditColorX&oldid=96567](https://wiki.resonite.com/index.php?title=Component:ButtonEditColorX&oldid=96567)"

Contents