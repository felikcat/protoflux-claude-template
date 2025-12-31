# Component:VirtualShiftColorDriver

> Source: https://wiki.resonite.com/Component:VirtualShiftColorDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f5/VirtualShiftColorDriverComponent.png/510px-VirtualShiftColorDriverComponent.png)](https://wiki.resonite.com/File:VirtualShiftColorDriverComponent.png) **Virtual Shift Color Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VirtualShiftColorDriver** component is used to change a color field whenever a keyboard specified has its Shift key state changed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Keyboard` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [VirtualKeyboard](https://wiki.resonite.com/Component:VirtualKeyboard "Component:VirtualKeyboard") >** | The keyboard to monitor the shirt state for. |
| `ColorTarget` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The field to set the color of depending on keyboard state. |
| `NormalColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to set the field in `ColorTarget` to when `Keyboard` is in default state. |
| `ShiftColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to set the field in `ColorTarget` to when `Keyboard`'s Shift key is toggled on like capslock. |
| `HoldColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to set the field in `ColorTarget` to when `Keyboard`'s Shift key is being held down. |

Fields
Collapse

## Usage

Provide values for all the fields in this component in order for it to start working.

## Examples

Used to make keys on the default keyboard change color when Shift is held, toggled, or released.

## See Also

- [Component:VirtualKey](https://wiki.resonite.com/Component:VirtualKey "Component:VirtualKey")
- [Component:VirtualKeyboard](https://wiki.resonite.com/Component:VirtualKeyboard "Component:VirtualKeyboard")
- [Component:VirtualModifierKey](https://wiki.resonite.com/Component:VirtualModifierKey "Component:VirtualModifierKey")
- [Component:VirtualMultiKey](https://wiki.resonite.com/Component:VirtualMultiKey "Component:VirtualMultiKey")
- [Component:VirtualShift](https://wiki.resonite.com/Component:VirtualShift "Component:VirtualShift")
- [Component:VirtualCloseKey](https://wiki.resonite.com/Component:VirtualCloseKey "Component:VirtualCloseKey")
- [Component:VirtualKeyTextDrive](https://wiki.resonite.com/Component:VirtualKeyTextDrive "Component:VirtualKeyTextDrive")
- Component:VirtualShiftColorDriver
- [Component:SimpleVirtualKeyboard](https://wiki.resonite.com/Component:SimpleVirtualKeyboard "Component:SimpleVirtualKeyboard")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VirtualShiftColorDriver&oldid=95846](https://wiki.resonite.com/index.php?title=Component:VirtualShiftColorDriver&oldid=95846)"

Contents