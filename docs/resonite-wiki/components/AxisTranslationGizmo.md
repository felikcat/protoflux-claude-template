# Component:AxisTranslationGizmo

> Source: https://wiki.resonite.com/Component:AxisTranslationGizmo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AxisTranslationGizmo&diff=96217) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fc/AxisTranslationGizmoComponent.png/510px-AxisTranslationGizmoComponent.png)](https://wiki.resonite.com/File:AxisTranslationGizmoComponent.png) **Axis Translation Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AxisTranslationGizmo** is the squares often seen on a Gizmo to translate it along 2 axies at the same time.

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
| `Axis` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction of the 2d plane this will translate along. |
| `AxisSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space of `Axis`. |
| `PointSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space of `TargetPoint` drive value. |
| `TargetPoint` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >>** | A field to drive with the target point position. |
| `TargetValue` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field to use for `TargetPoint` |
| `UseCustomVisual` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use a custom visual rather than the default code generated one. |
| `_customVisualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the custom visual. |
| `ArrowLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The length of the arrow this gizmo is attached to. |
| `CreateUndoSteps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to make edits done with this component undoable. |
| `_visualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the visual for interaction. |
| `_visualRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the visual. |
| `_arrowVector` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The vector field of the arrow mesh visual. |
| `_arrow` | **[ArrowMesh](https://wiki.resonite.com/Component:ArrowMesh "Component:ArrowMesh")** | The arrow mesh of the visual. |
| `_collider` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[CylinderCollider](https://wiki.resonite.com/Component:CylinderCollider "Component:CylinderCollider")** | The collider of the visual. |
| `_linesRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the root slot of the lines visual. |
| `_line0` | **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The segment mesh being used for the first line. |
| `_line1` | **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The segment mesh being used for the second line. |

Fields
Collapse

## Usage

Used For Gizmos.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AxisTranslationGizmo&oldid=96217](https://wiki.resonite.com/index.php?title=Component:AxisTranslationGizmo&oldid=96217)"

Contents