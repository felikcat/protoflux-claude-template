# Component:VirtualKeyTextDrive

> Source: https://wiki.resonite.com/Component:VirtualKeyTextDrive

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d0/VirtualKeyTextDriveComponent.png/510px-VirtualKeyTextDriveComponent.png)](https://wiki.resonite.com/File:VirtualKeyTextDriveComponent.png) **Virtual Key Text Drive** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component takes a [VirtualKey](https://wiki.resonite.com/Component:VirtualKey "Component:VirtualKey") component and uses it's settings to drive a textfield's content to match what that key would type when pressed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Key` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [VirtualKey](https://wiki.resonite.com/Component:VirtualKey "Component:VirtualKey") >** | The virtual key to source the text from (so if the virtual key is set to "d" it will drive the target of `Text` to "d". |
| `Text` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text field to drive |

Fields
Collapse

## Examples

Used in keys in the default keyboard to change the keys to capital letters when shift or caps is enabled.

## See Also

- [Component:VirtualKey](https://wiki.resonite.com/Component:VirtualKey "Component:VirtualKey")
- [Component:VirtualKeyboard](https://wiki.resonite.com/Component:VirtualKeyboard "Component:VirtualKeyboard")
- [Component:VirtualModifierKey](https://wiki.resonite.com/Component:VirtualModifierKey "Component:VirtualModifierKey")
- [Component:VirtualMultiKey](https://wiki.resonite.com/Component:VirtualMultiKey "Component:VirtualMultiKey")
- [Component:VirtualShift](https://wiki.resonite.com/Component:VirtualShift "Component:VirtualShift")
- [Component:VirtualCloseKey](https://wiki.resonite.com/Component:VirtualCloseKey "Component:VirtualCloseKey")
- Component:VirtualKeyTextDrive
- [Component:VirtualShiftColorDriver](https://wiki.resonite.com/Component:VirtualShiftColorDriver "Component:VirtualShiftColorDriver")
- [Component:SimpleVirtualKeyboard](https://wiki.resonite.com/Component:SimpleVirtualKeyboard "Component:SimpleVirtualKeyboard")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VirtualKeyTextDrive&oldid=95659](https://wiki.resonite.com/index.php?title=Component:VirtualKeyTextDrive&oldid=95659)"

Contents