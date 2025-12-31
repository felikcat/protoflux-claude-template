# Component:ScaleGizmo

> Source: https://wiki.resonite.com/Component:ScaleGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4d/ScaleGizmoComponent.png/510px-ScaleGizmoComponent.png)](https://wiki.resonite.com/File:ScaleGizmoComponent.png) **Scale Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScaleGizmo** component is used to allow scaling of a slot it is targeting.

See [Dev tool](https://wiki.resonite.com/Dev_tool "Dev tool").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetSlot` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The slot this is scaling/targeting. |
| `AutoPositionAtTargetSlot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to auto position this gizmo at `TargetSlot` |
| `_interactingComponent` | **[Component](https://wiki.resonite.com/Type:Component "Type:Component")** | The component that is interacting with this component. |
| `_material` | **[OverlayFresnelMaterial](https://wiki.resonite.com/OverlayFresnelMaterial "OverlayFresnelMaterial")** | The material for the gizmo visual. |
| `_toolPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot representing the interacting dev tool's tip. |
| `_activePoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The active point of the gizmo |
| `_lineRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the root of the line visual going back to `_toolPoint`. |
| `_lineSegment` | **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The line segment for the line from gizmo center to `_toolPoint`. |
| `_snapHighlight` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot for a snap point highlight like a selected cube corner. |
| `TargetScale` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The scale field of what this is scaling. |
| `HandleLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The length of the scale gizmo handles. |
| `_xSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The scale gizmo for the x axis. |
| `_ySlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The scale gizmo for the y axis. |
| `_zSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The scale gizmo for the z axis. |

Fields
Collapse

## Usage

See [Dev tool](https://wiki.resonite.com/Dev_tool "Dev tool").

## Examples

See [Dev tool](https://wiki.resonite.com/Dev_tool "Dev tool").

## See Also

- [Dev tool](https://wiki.resonite.com/Dev_tool "Dev tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScaleGizmo&oldid=106546](https://wiki.resonite.com/index.php?title=Component:ScaleGizmo&oldid=106546)"

Contents