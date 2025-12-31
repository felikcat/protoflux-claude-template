# Component:ColorXMemberEditor

> Source: https://wiki.resonite.com/Component:ColorXMemberEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/cf/ColorXMemberEditorComponent.png/510px-ColorXMemberEditorComponent.png)](https://wiki.resonite.com/File:ColorXMemberEditorComponent.png) **ColorX Member Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorXMemberEditor** component is used in [inspectors](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") and [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking") to edit [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") Fields and their [UIX](https://wiki.resonite.com/UIX "UIX") elements.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you just want to change a color with a press of a button, use [ButtonEditColorX](https://wiki.resonite.com/Component:ButtonEditColorX "Component:ButtonEditColorX") instead.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Continuous` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether updates to the target are continuous. |
| `_path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Usually "r" "g" "b" "a" to edit parts of the colorX value. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | The colorX to edit. |
| `Labels` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show field labels. |
| `Vertical` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the inspector showing this component is showing it in a vertical fashion. |
| `_colorDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive with the colorX color for the inspector visual. |
| `_colorDriveNoAlpha` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive with the colorX target with no alpha applied for the inspector visual. |
| `_colorDialog` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface") >** | The color dialogue currently being used to edit the color. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OpenColorPicker:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles spawning the user's favorite color picker so they can edit this component's target color. |

Triggers
Collapse

## Usage

Internal.

## Examples

Used in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") where colors are on Components so the user can edit the colors.

## See Also

- [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")
- [Type:colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")
- [Component:ButtonEditColorX](https://wiki.resonite.com/Component:ButtonEditColorX "Component:ButtonEditColorX")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorXMemberEditor&oldid=98348](https://wiki.resonite.com/index.php?title=Component:ColorXMemberEditor&oldid=98348)"

Contents