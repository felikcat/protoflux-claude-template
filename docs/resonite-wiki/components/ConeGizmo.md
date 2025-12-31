# Component:ConeGizmo

> Source: https://wiki.resonite.com/Component:ConeGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4f/ConeGizmoComponent.png/510px-ConeGizmoComponent.png)](https://wiki.resonite.com/File:ConeGizmoComponent.png) **Cone Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ConeGizmo** component is auto generated for interaction with a [Component:ConeMesh](https://wiki.resonite.com/Component:ConeMesh "Component:ConeMesh") or [Component:ConeCollider](https://wiki.resonite.com/Component:ConeCollider "Component:ConeCollider") via a [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool").

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
| `TargetAngle` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field being edited for the angle of the cone. |
| `TargetRadius` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field being edited for the radius of the cone base. |
| `TargetHeight` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field being edited for the height of the cone. |
| `TargetDirection` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >>** | The field being edited for the cone direction. |
| `TargetRotation` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >>** | The field being edited for the cone rotation. |
| `DirectionSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space Transform of `TargetDirection`. |
| `FixedAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle that the cone should be at (shape). |
| `FixedHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height that the cone mesh should be. |
| `FixedDirection` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction the cone should be facing. |
| `LineThickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of the lines of the visual. |
| `MinHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum height the cone can be set to. |
| `MaxHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum height the cone can be set to. |
| `MinAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum tip angle the cone can be set to (shape). |
| `MaxAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum tip angle the cone can be set to (shape). |
| `_visualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the visual for this gizmo. |
| `_visualRot` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the `_visualRoot` slot. |
| `_handles` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ConeGizmo.Handle](https://wiki.resonite.com/Component:ConeGizmo#Handle)** | A list of Handle objects this cone gizmo has. |
| `_heightMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The mesh being used to signal the height of the cone. |
| `_coneLineMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The line segment based mesh that shows the cone itself. |

Fields
Collapse

## Handle

| Name | Type | Description |
| --- | --- | --- |
| `RelativeHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The relative height of this handle compared to the cone. |
| `root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the visual and interface of this handle. |
| `offset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the offset of the handle. |
| `mesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[TorusMesh](https://wiki.resonite.com/Component:TorusMesh "Component:TorusMesh")** | The mesh being used for this handle. |

Fields

## Usage

Generated automatically.

## Examples

Used for interacting with cone objects via the [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool").

## See Also

- [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool")
- [Gizmo](https://wiki.resonite.com/Gizmo "Gizmo")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConeGizmo&oldid=101401](https://wiki.resonite.com/index.php?title=Component:ConeGizmo&oldid=101401)"

Contents