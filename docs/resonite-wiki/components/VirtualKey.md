# Component:VirtualKey

> Source: https://wiki.resonite.com/Component:VirtualKey

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a0/VirtualKeyComponent.png/510px-VirtualKeyComponent.png)](https://wiki.resonite.com/File:VirtualKeyComponent.png) **Virtual Key** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Virtual key is a component that turns a [button event](https://wiki.resonite.com/Button_Events "Button Events") into a button press on the keyboard in game as if it came from the physical keyboard.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetKey` | **[Key](https://wiki.resonite.com/Type:Key "Type:Key")** | The key to simulate. |
| `AppendString` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | What text to append if the user is focused into a text field |
| `ShiftTargetKey` | **[Key](https://wiki.resonite.com/Type:Key "Type:Key")** | What key to use if the [Virtual Shift component](https://wiki.resonite.com/Component:VirtualShift "Component:VirtualShift") is taking effect, or shift is held on the physical keyboard. |
| `ShiftAppendString` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | What text to append if the user is focused into a text field and if the [Virtual Shift component](https://wiki.resonite.com/Component:VirtualShift "Component:VirtualShift") is taking effect, or shift is held on the physical keyboard. |
| `IgnoreShift` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to ignore shift and virtual shift keys entirely. |
| `ModifierKey` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [VirtualModifierKey](https://wiki.resonite.com/Component:VirtualModifierKey "Component:VirtualModifierKey") >** | A key that can act as a special modifier (for example, if you wanted a key on your VR keyboard that appended "Cat!!" every time you type a letter) |
| `ModifiedTargetKey` | **[Key](https://wiki.resonite.com/Type:Key "Type:Key")** | The key to use instead of `TargetKey` when `ModifiedTargetKey` is pressed down. |
| `ModifiedAppendString` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | hat text to append if the user is focused into a text field and the key specified by `ModifiedTargetKey` is pressed down. |
| `Keyboard` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [VirtualKeyboard](https://wiki.resonite.com/Component:VirtualKeyboard "Component:VirtualKeyboard") >** | The keyboard object this key is a part of. |

Fields
Collapse

## Behavior

When paired with a UIX button or physical button on the same slot, it allows for simulation of key presses as if they came from the actual physical keyboard. This can be used for some funny effects where pressing a button forces the user that pressed it to jump (or, god forbid, make them switch to desktop or VR)

This cannot be used to send key presses outside of Resonite to control the external operating system unless the component is in [Userspace](https://wiki.resonite.com/Userspace "Userspace").

## Examples

Used in the default and custom community keyboards to allow said keyboards to type into the game and textfields.

## See Also

- Component:VirtualKey
- [Component:VirtualKeyboard](https://wiki.resonite.com/Component:VirtualKeyboard "Component:VirtualKeyboard")
- [Component:VirtualModifierKey](https://wiki.resonite.com/Component:VirtualModifierKey "Component:VirtualModifierKey")
- [Component:VirtualMultiKey](https://wiki.resonite.com/Component:VirtualMultiKey "Component:VirtualMultiKey")
- [Component:VirtualShift](https://wiki.resonite.com/Component:VirtualShift "Component:VirtualShift")
- [Component:VirtualCloseKey](https://wiki.resonite.com/Component:VirtualCloseKey "Component:VirtualCloseKey")
- [Component:VirtualKeyTextDrive](https://wiki.resonite.com/Component:VirtualKeyTextDrive "Component:VirtualKeyTextDrive")
- [Component:VirtualShiftColorDriver](https://wiki.resonite.com/Component:VirtualShiftColorDriver "Component:VirtualShiftColorDriver")
- [Component:SimpleVirtualKeyboard](https://wiki.resonite.com/Component:SimpleVirtualKeyboard "Component:SimpleVirtualKeyboard")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VirtualKey&oldid=95663](https://wiki.resonite.com/index.php?title=Component:VirtualKey&oldid=95663)"

Contents