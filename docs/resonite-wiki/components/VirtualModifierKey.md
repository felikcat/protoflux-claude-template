# Component:VirtualModifierKey

> Source: https://wiki.resonite.com/Component:VirtualModifierKey

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d9/VirtualModifierKeyComponent.png/510px-VirtualModifierKeyComponent.png)](https://wiki.resonite.com/File:VirtualModifierKeyComponent.png) **Virtual Modifier Key** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Virtual Modifier Key is a way of making [Virtual Keys](https://wiki.resonite.com/Component:VirtualKey "Component:VirtualKey") change what they type when pressed.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Keyboard` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [VirtualKeyboard](https://wiki.resonite.com/Component:VirtualKeyboard "Component:VirtualKeyboard") >** | The keyboard this key is a part of. |
| `State` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this modifier key is active or not, kind of like if CAPSLOCK was active. |

Fields
Collapse

## Examples

This can be used to make a button that when activated, makes all the keys on the VR keyboard append "CHEESE!" whenever a key is pressed. Keep in mind the key would need to be a part of a saved [favorite](https://wiki.resonite.com/Favorites "Favorites") keyboard.

## See Also

- [Component:VirtualKey](https://wiki.resonite.com/Component:VirtualKey "Component:VirtualKey")
- [Component:VirtualKeyboard](https://wiki.resonite.com/Component:VirtualKeyboard "Component:VirtualKeyboard")
- Component:VirtualModifierKey
- [Component:VirtualMultiKey](https://wiki.resonite.com/Component:VirtualMultiKey "Component:VirtualMultiKey")
- [Component:VirtualShift](https://wiki.resonite.com/Component:VirtualShift "Component:VirtualShift")
- [Component:VirtualCloseKey](https://wiki.resonite.com/Component:VirtualCloseKey "Component:VirtualCloseKey")
- [Component:VirtualKeyTextDrive](https://wiki.resonite.com/Component:VirtualKeyTextDrive "Component:VirtualKeyTextDrive")
- [Component:VirtualShiftColorDriver](https://wiki.resonite.com/Component:VirtualShiftColorDriver "Component:VirtualShiftColorDriver")
- [Component:SimpleVirtualKeyboard](https://wiki.resonite.com/Component:SimpleVirtualKeyboard "Component:SimpleVirtualKeyboard")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VirtualModifierKey&oldid=95657](https://wiki.resonite.com/index.php?title=Component:VirtualModifierKey&oldid=95657)"

Contents