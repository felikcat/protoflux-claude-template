# Component:EnumMemberEditor

> Source: https://wiki.resonite.com/Component:EnumMemberEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c2/EnumMemberEditorComponent.png/510px-EnumMemberEditorComponent.png)](https://wiki.resonite.com/File:EnumMemberEditorComponent.png) **Enum Member Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **EnumMemberEditor** component is used in inspectors to edit enum values.

Commonly used in [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking") if interacted with directly by the user instead of as part of an inspector visual.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Continuous` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether changes should be continuous and instant. |
| `_path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The sub path of the value type to edit. |
| `_target` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | The field to edit and get info from. |
| `_textDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text field to drive with the enum's contents. |
| `_button` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to edit the enum with. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `DecrementEnum:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Goes up by 1 in the enum values. |
| `IncrementEnum:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Goes down by 1 in the enum values. |

Triggers
Collapse

## Usage

Not used directly by the user.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:EnumMemberEditor&oldid=98444](https://wiki.resonite.com/index.php?title=Component:EnumMemberEditor&oldid=98444)"

Contents