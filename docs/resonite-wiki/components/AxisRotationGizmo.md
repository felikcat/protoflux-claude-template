# Component:AxisRotationGizmo

> Source: https://wiki.resonite.com/Component:AxisRotationGizmo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AxisRotationGizmo&diff=96224) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/41/AxisRotationGizmoComponent.png/510px-AxisRotationGizmoComponent.png)](https://wiki.resonite.com/File:AxisRotationGizmoComponent.png) **Axis Rotation Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AxisRotationGizmo** component is used for one of the any 3 axies of rotation for a rotation gizmo that can be interacted with through the [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetSlot` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The slot to translate and edit. |
| `AutoPositionAtTargetSlot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to automatically position this at the target slot. |
| `_interactingComponent` | **[Component](https://wiki.resonite.com/Type:Component "Type:Component")** | the component This is interacting with. |
| `_material` | **[OverlayFresnelMaterial](https://wiki.resonite.com/OverlayFresnelMaterial "OverlayFresnelMaterial")** | The material being used for the visual. |
| `_toolPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The point that follows the interacting tool's tip. |
| `_activePoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The point that follows the gizmo visual. |
| `_lineRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the root of the line visual from the gizmo to the interacting tool's tip. |
| `_lineSegment` | **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The segment mesh being used for the line visual. |
| `_snapHighlight` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the root of the snap highlight for snapping. |
| `Axis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction of the 2d axis this will rotate along. |
| `AxisSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space of `Axis`. |
| `RotationSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space of the `TargetRotation` drive target. |
| `TargetRotation` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >>** | A field to drive with the target rotation |
| `TargetValue` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field to drive `TargetRotation` with. |
| `CircleRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the rotation circle gizmo. |
| `CircleThickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of the torus of the rotation gizmo. |
| `_visualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the visual for interaction. |
| `_visualRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the visual. |
| `_circle` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[TorusMesh](https://wiki.resonite.com/Component:TorusMesh "Component:TorusMesh")** | The torus mesh being used to make the rotation gizmo interact visual. |
| `_circleColliderMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[TorusMesh](https://wiki.resonite.com/Component:TorusMesh "Component:TorusMesh")** | The collider for the circle rotation gizmo visual. |
| `_referenceLine` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The reference line mesh component. |
| `_linesRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the visuals for the lines. |
| `_line0` | **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The line along the rotation plane to below the tooltip. |
| `_line1` | **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The line from the end of `_line0` to the tooltip. |

Fields
Collapse

## Usage

Used for Gizmos.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AxisRotationGizmo&oldid=96224](https://wiki.resonite.com/index.php?title=Component:AxisRotationGizmo&oldid=96224)"

Contents