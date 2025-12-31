# Component:ColorMemberEditor

> Source: https://wiki.resonite.com/Component:ColorMemberEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4d/ColorMemberEditorComponent.png/510px-ColorMemberEditorComponent.png)](https://wiki.resonite.com/File:ColorMemberEditorComponent.png) **Color Member Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorMemberEditor** component is used in inspectors and [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking") to edit Color Fields and their elements.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Continuous` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether updates to the target are continuous. |
| `_path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Usually "r" "g" "b" "a" to edit parts of the color value. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | The color to edit. |
| `Labels` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show field labels. |
| `Vertical` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the inspector showing this component is showing it in a vertical fashion. |
| `_colorDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive with the color value for the inspector visual. |
| `_colorDriveNoAlpha` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive with the color target with no alpha applied for the inspector visual. |
| `_colorDialog` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface") >** | The color dialogue currently being used to edit the color. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OpenColorPicker:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles opening and spawning the user's favorite color picker for editing the color via a picker. |

Triggers
Collapse

## Usage

Internal.

## Examples

Used in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") where colors are on Components so the user can edit the colors.

## See Also

- [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")
- [Type:Color](https://wiki.resonite.com/Type:Color "Type:Color")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorMemberEditor&oldid=98345](https://wiki.resonite.com/index.php?title=Component:ColorMemberEditor&oldid=98345)"

Contents