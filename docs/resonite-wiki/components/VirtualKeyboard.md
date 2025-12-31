# Component:VirtualKeyboard

> Source: https://wiki.resonite.com/Component:VirtualKeyboard

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/00/VirtualKeyboardComponent.png/510px-VirtualKeyboardComponent.png)](https://wiki.resonite.com/File:VirtualKeyboardComponent.png) **Virtual Keyboard** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The Virtual Keyboard is a component that groups many [Keys](https://wiki.resonite.com/Component:VirtualKey "Component:VirtualKey"), [Modifier Keys](https://wiki.resonite.com/Component:VirtualModifierKey "Component:VirtualModifierKey"), and [Multi Keys](https://wiki.resonite.com/Component:VirtualMultiKey "Component:VirtualMultiKey") together.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ShiftActive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the [Virtual Shift](https://wiki.resonite.com/Component:VirtualShift "Component:VirtualShift") key is toggled to pressed. |
| `HoldShift` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the [Virtual Shift](https://wiki.resonite.com/Component:VirtualShift "Component:VirtualShift") key is held. |
| `TextPreviewActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | drives the visibility of the preview text display. |
| `TextPreview` | **[IText](https://wiki.resonite.com/Type:IText "Type:IText")** | The text preview object that shows what the user is typing. |

Fields
Collapse

## Examples

Used in the default keyboard every user comes with, and

## See Also

- [Component:VirtualKey](https://wiki.resonite.com/Component:VirtualKey "Component:VirtualKey")
- Component:VirtualKeyboard
- [Component:VirtualModifierKey](https://wiki.resonite.com/Component:VirtualModifierKey "Component:VirtualModifierKey")
- [Component:VirtualMultiKey](https://wiki.resonite.com/Component:VirtualMultiKey "Component:VirtualMultiKey")
- [Component:VirtualShift](https://wiki.resonite.com/Component:VirtualShift "Component:VirtualShift")
- [Component:VirtualCloseKey](https://wiki.resonite.com/Component:VirtualCloseKey "Component:VirtualCloseKey")
- [Component:VirtualKeyTextDrive](https://wiki.resonite.com/Component:VirtualKeyTextDrive "Component:VirtualKeyTextDrive")
- [Component:VirtualShiftColorDriver](https://wiki.resonite.com/Component:VirtualShiftColorDriver "Component:VirtualShiftColorDriver")
- [Component:SimpleVirtualKeyboard](https://wiki.resonite.com/Component:SimpleVirtualKeyboard "Component:SimpleVirtualKeyboard")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VirtualKeyboard&oldid=95661](https://wiki.resonite.com/index.php?title=Component:VirtualKeyboard&oldid=95661)"

Contents