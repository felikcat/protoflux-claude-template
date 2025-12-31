# Component:VirtualMultiKey

> Source: https://wiki.resonite.com/Component:VirtualMultiKey

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/94/VirtualMultiKeyComponent.png/510px-VirtualMultiKeyComponent.png)](https://wiki.resonite.com/File:VirtualMultiKeyComponent.png) **Virtual Multi Key** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component when triggered by a [button event](https://wiki.resonite.com/Button_Events "Button Events") will make the user press all the keys in the multikey at the same time.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Keys` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Key](https://wiki.resonite.com/Type:Key "Type:Key") >** | A list of keys that should be simulated being pressed when receiving a [button event](https://wiki.resonite.com/Button_Events "Button Events") and they will be simulated by the source user of the button event. |

Fields
Collapse

## Behavior

The keys do not press in order, and keys will not be pressed more than once if listed more than once.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:VirtualKey](https://wiki.resonite.com/Component:VirtualKey "Component:VirtualKey")
- [Component:VirtualKeyboard](https://wiki.resonite.com/Component:VirtualKeyboard "Component:VirtualKeyboard")
- [Component:VirtualModifierKey](https://wiki.resonite.com/Component:VirtualModifierKey "Component:VirtualModifierKey")
- Component:VirtualMultiKey
- [Component:VirtualShift](https://wiki.resonite.com/Component:VirtualShift "Component:VirtualShift")
- [Component:VirtualCloseKey](https://wiki.resonite.com/Component:VirtualCloseKey "Component:VirtualCloseKey")
- [Component:VirtualKeyTextDrive](https://wiki.resonite.com/Component:VirtualKeyTextDrive "Component:VirtualKeyTextDrive")
- [Component:VirtualShiftColorDriver](https://wiki.resonite.com/Component:VirtualShiftColorDriver "Component:VirtualShiftColorDriver")
- [Component:SimpleVirtualKeyboard](https://wiki.resonite.com/Component:SimpleVirtualKeyboard "Component:SimpleVirtualKeyboard")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VirtualMultiKey&oldid=95660](https://wiki.resonite.com/index.php?title=Component:VirtualMultiKey&oldid=95660)"

Contents