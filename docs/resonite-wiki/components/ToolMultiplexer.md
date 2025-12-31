# Component:ToolMultiplexer

> Source: https://wiki.resonite.com/Component:ToolMultiplexer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/87/ToolMultiplexerComponent.png/510px-ToolMultiplexerComponent.png)](https://wiki.resonite.com/File:ToolMultiplexerComponent.png) **Tool Multiplexer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A Tool Multiplexer is a key component in almost every [multitool](https://wiki.resonite.com/Tools#MultiTools "Tools") to ever exist. It handles the switching and usage of multiple tools, and allows all of them to act as one tool tip the user can equip, making multiple tool usage easier. Multitools can be assigned to the `Tools` list of other multitools.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_equipLink` | _direct_ **[LinkTarget\`1](https://wiki.resonite.com/index.php?title=Type:LinkTarget%601&action=edit&redlink=1 "Type:LinkTarget`1 (page does not exist)") < [ITool](https://wiki.resonite.com/Type:ITool "Type:ITool") >** | This is Internal, and is used by the engine to retrieve the component this field is a part of. It cannot be assigned to. |
| `TipReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to use as the tool's tip, instead of the component's slot. |
| `BlockGripEquip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to prevent legacy double grip equipping from equipping this tooltip. |
| `BlockRemoteEquip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to prevent equipping by clicking via laser |
| `EquipName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the tool in the context menu when equipping via context menu. |
| `_overrideActiveTool` | **[InteractionHandler](https://wiki.resonite.com/Component:InteractionHandler "Component:InteractionHandler")** | The interaction handler to use instead of this tool as an interaction handler. |
| `_gripPosesGenerated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the [Grip Pose Reference](https://wiki.resonite.com/Component:GripPoseReference "Component:GripPoseReference") components and slots have been generated for this tool. |
| `ActiveToolIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The tool that this tool tip is currently using |
| `Tools` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[ITool](https://wiki.resonite.com/Type:ITool "Type:ITool")** | A list of tools that this tool tip is to switch between using `ActiveToolIndex` as the one it should be currently using. |

Fields
Collapse

## Behavior

Curiously, the transform position of the slot of a tool listed in the `Tools` list and its tip transform position can cause the multitool's laser tip to move if that tool is selected. Putting all the tools used by the multitool under one slot and making sure their tip and tool roots are in the same transform place is the preferred way of making sure your tool tip laser position stays consistent.

## Examples

From [Uki's](https://wiki.resonite.com/index.php?title=User:Ukilop&action=edit&redlink=1 "User:Ukilop (page does not exist)") Redprint tip, to the default multitool in [Resonite Essentials](https://wiki.resonite.com/Resonite_Essentials "Resonite Essentials") to H3's tool, this component is vital in a multitool, and what makes them function.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ToolMultiplexer&oldid=106523](https://wiki.resonite.com/index.php?title=Component:ToolMultiplexer&oldid=106523)"

Contents