# Component:MeshTool

> Source: https://wiki.resonite.com/Component:MeshTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/85/MeshToolComponent.png/510px-MeshToolComponent.png)](https://wiki.resonite.com/File:MeshToolComponent.png) **Mesh Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Mesh Tool](https://wiki.resonite.com/Mesh_Tool "Mesh Tool").

## Fields

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
| `_orbSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The place to put a grabbed mesh orb. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SnapFilter:Func`3<Snapper, SnapTarget, Bool>`` | **[Func\`3](https://wiki.resonite.com/Type:Func%603 "Type:Func`3") < [Snapper](https://wiki.resonite.com/Component:Snapper "Component:Snapper"), [SnapTarget](https://wiki.resonite.com/Component:SnapTarget "Component:SnapTarget"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | ✓ | Can be used as a function to filter snappers so they accept only specific snappers. In this case, it will only accept mesh orbs. |
| `EditMesh:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the edit mesh button is touched. |

Triggers
Collapse

## Usage

See [Mesh Tool](https://wiki.resonite.com/Mesh_Tool "Mesh Tool").

## Examples

See [Mesh Tool](https://wiki.resonite.com/Mesh_Tool "Mesh Tool").

## See Also

- [Mesh Tool](https://wiki.resonite.com/Mesh_Tool "Mesh Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshTool&oldid=99077](https://wiki.resonite.com/index.php?title=Component:MeshTool&oldid=99077)"

Contents