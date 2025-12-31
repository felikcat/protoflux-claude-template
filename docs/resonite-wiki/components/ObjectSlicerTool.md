# Component:ObjectSlicerTool

> Source: https://wiki.resonite.com/Component:ObjectSlicerTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/04/ObjectSlicerToolComponent.png/510px-ObjectSlicerToolComponent.png)](https://wiki.resonite.com/File:ObjectSlicerToolComponent.png) **Object Slicer Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Object Slicer Tool](https://wiki.resonite.com/Object_Slicer_Tool "Object Slicer Tool").

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
| `ApplyToObjectRoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the slicing material effect should be applied to the nearest object root. |
| `EdgeColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | what the edge color for new generated slice materials should be. |
| `EdgeStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The start of the range of the edge color from the slicer. |
| `EdgeEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The end of the range of the edge color from the slicer. |
| `_slicers` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[GenericSlicer](https://wiki.resonite.com/Component:GenericSlicer "Component:GenericSlicer")** | The list of slicers this tool has generated and/or is controlling. |
| `_sliceMaterials` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[PBS\_Slice](https://wiki.resonite.com/Type:PBS_Slice "Type:PBS Slice")** | The list of slice materials this tool has generated and/or is controlling. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `CreateSlicer:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the create slicer button is touched. |
| `ClearSetup:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the clear setup button is touched. |

Triggers
Collapse

## Usage

See [Object Slicer Tool](https://wiki.resonite.com/Object_Slicer_Tool "Object Slicer Tool").

## Examples

See [Object Slicer Tool](https://wiki.resonite.com/Object_Slicer_Tool "Object Slicer Tool").

## See Also

- [Object Slicer Tool](https://wiki.resonite.com/Object_Slicer_Tool "Object Slicer Tool")
- [Type:PBS\_Slice](https://wiki.resonite.com/Type:PBS_Slice "Type:PBS Slice")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ObjectSlicerTool&oldid=99084](https://wiki.resonite.com/index.php?title=Component:ObjectSlicerTool&oldid=99084)"

Contents