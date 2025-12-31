# Component:MeterTool

> Source: https://wiki.resonite.com/Component:MeterTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2a/MeterToolComponent.png/510px-MeterToolComponent.png)](https://wiki.resonite.com/File:MeterToolComponent.png) **Meter Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Meter Tool](https://wiki.resonite.com/Meter_Tool "Meter Tool").

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
| `_indicationColor` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The field to change the color value for when doing status indications. |
| `MeterMode` | **[MeterTool.Mode](https://wiki.resonite.com/Component:MeterTool#Mode)** | The mode the tool is currently in. |
| `MeasureInObjectSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If measurements should be done in global space or parent space. |
| `RaycastIgnoresUsers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the tool raycast ignores colliders with an active user. |
| `MultiPoint` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Measure between two points, or any amount of points. |
| `_lastPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot of the last point placed by the tool. |
| `_currentMeter` | **[DistanceMeter](https://wiki.resonite.com/Component:DistanceMeter "Component:DistanceMeter")** | The current object displaying the distance between points. |
| `_currentLineTransform` | **[LineTransform](https://wiki.resonite.com/Component:LineTransform "Component:LineTransform")** | The current line transform object being used to display the distance between points |
| `FormatNumber` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | How to format the numbers. |
| `FormatUnit` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | How to format the units. |

Fields
Collapse

## Mode

| Name | Value | Description |
| --- | --- | --- |
| `Ray` | 0 | Shoots a ray from the tip of the tool and places a point wherever it hits. |
| `Perpendicular` | 1 | Shoots a ray up from where the first point is placed. |
| `Drag` | 2 | Puts points between where you start and stop dragging. |

Values

## Usage

See [Meter Tool](https://wiki.resonite.com/Meter_Tool "Meter Tool").

## Examples

See [Meter Tool](https://wiki.resonite.com/Meter_Tool "Meter Tool").

## See Also

- [Meter Tool](https://wiki.resonite.com/Meter_Tool "Meter Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeterTool&oldid=97623](https://wiki.resonite.com/index.php?title=Component:MeterTool&oldid=97623)"

Contents