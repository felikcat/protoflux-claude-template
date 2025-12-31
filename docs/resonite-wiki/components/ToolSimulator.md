# Component:ToolSimulator

> Source: https://wiki.resonite.com/Component:ToolSimulator

Collapse **Component image**

[![](https://wiki.resonite.com/images/8/87/ToolSimulatorComponent.jpg)](https://wiki.resonite.com/File:ToolSimulatorComponent.jpg) **Tool Simulator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The ToolSimulator [Component](https://wiki.resonite.com/Component "Component") allows a tool to be used without needing it to be equipped by a [User](https://wiki.resonite.com/User "User"). You can make use of a [Tool's](https://wiki.resonite.com/Tools "Tools") primary and secondary actions but not context menu actions.

You need to provide a [reference](https://wiki.resonite.com/Reference "Reference") to the tool component that you want to simulate, and also a reference to a simulating user. You can then make use of the Primary, Secondary, Strength and Axis properties.

For example, providing a reference to a [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool") and then making use of the Primary property will allow you to apply [materials](https://wiki.resonite.com/Material "Material") to objects in front of the tool.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Tool` | **[ITool](https://wiki.resonite.com/Type:ITool "Type:ITool")** | The tool to simulate the use of. |
| `SimulatingUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that should simulate the tool. |
| `Primary` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Tool` should be simulated as holding primary. |
| `Secondary` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Tool` should be simulated as holding secondary. |
| `Strength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The primary strength the `Tool` should be simulated as using. |
| `Axis` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The position axis (like trackpad) the `Tool` should be simulated as using. |

Fields
Collapse

## Known Bugs

Currently the primary of the [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool") is not simulated properly and can not move gizmos. [\[1\]](https://wiki.resonite.com/Component:ToolSimulator#cite_note-1)

## Usage

## Examples

## See Also

1. [↑](https://wiki.resonite.com/Component:ToolSimulator#cite_ref-1 "Jump up")[https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/3570](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/3570)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ToolSimulator&oldid=106592](https://wiki.resonite.com/index.php?title=Component:ToolSimulator&oldid=106592)"

Contents