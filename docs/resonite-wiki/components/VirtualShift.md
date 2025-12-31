# Component:VirtualShift

> Source: https://wiki.resonite.com/Component:VirtualShift

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8a/VirtualShiftComponent.png/510px-VirtualShiftComponent.png)](https://wiki.resonite.com/File:VirtualShiftComponent.png) **Virtual Shift** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Simulates pressing or holding onto the shift key on a normal physical keyboard.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Keyboard` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [VirtualKeyboard](https://wiki.resonite.com/Component:VirtualKeyboard "Component:VirtualKeyboard") >** | The keyboard which the keys should be set or unset from the holding shift state. |
| `HoldPressInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | what value `_lastPress` has to be below when the button is pressed again to enable `AlwaysHold` field. |
| `AlwaysHold` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user has double clicked shift and enabled a constant hold shift state. |
| `_lastPress` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | Internal, how many seconds has passed since this button was last pressed. is used to handle enabling/disabling `AlwaysHold` field. |

Fields
Collapse

## Examples

Is used in the default keyboard to make the shift key function.

## See Also

- [Component:VirtualKey](https://wiki.resonite.com/Component:VirtualKey "Component:VirtualKey")
- [Component:VirtualKeyboard](https://wiki.resonite.com/Component:VirtualKeyboard "Component:VirtualKeyboard")
- [Component:VirtualModifierKey](https://wiki.resonite.com/Component:VirtualModifierKey "Component:VirtualModifierKey")
- [Component:VirtualMultiKey](https://wiki.resonite.com/Component:VirtualMultiKey "Component:VirtualMultiKey")
- Component:VirtualShift
- [Component:VirtualCloseKey](https://wiki.resonite.com/Component:VirtualCloseKey "Component:VirtualCloseKey")
- [Component:VirtualKeyTextDrive](https://wiki.resonite.com/Component:VirtualKeyTextDrive "Component:VirtualKeyTextDrive")
- [Component:VirtualShiftColorDriver](https://wiki.resonite.com/Component:VirtualShiftColorDriver "Component:VirtualShiftColorDriver")
- [Component:SimpleVirtualKeyboard](https://wiki.resonite.com/Component:SimpleVirtualKeyboard "Component:SimpleVirtualKeyboard")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VirtualShift&oldid=95662](https://wiki.resonite.com/index.php?title=Component:VirtualShift&oldid=95662)"

Contents