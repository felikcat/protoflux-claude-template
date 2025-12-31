# Component:VectorGizmo

> Source: https://wiki.resonite.com/Component:VectorGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fc/VectorGizmoComponent.png/510px-VectorGizmoComponent.png)](https://wiki.resonite.com/File:VectorGizmoComponent.png) **Vector Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VectorGizmo** component is used to allow editing a gizmo via the [Dev tool](https://wiki.resonite.com/Dev_tool "Dev tool").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetSlot` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The slot to influence or a component this is on. |
| `AutoPositionAtTargetSlot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to position the gizmo at `TargetSlot`. |
| `_interactingComponent` | **[Component](https://wiki.resonite.com/Type:Component "Type:Component")** | The component like a [Dev tool](https://wiki.resonite.com/Dev_tool "Dev tool") that is interacting with this gizmo. |
| `_material` | **[OverlayFresnelMaterial](https://wiki.resonite.com/OverlayFresnelMaterial "OverlayFresnelMaterial")** | The material being used for the gizmo visual. |
| `_toolPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to position at the interacting tool's tip slot. |
| `_activePoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to position at the active point. |
| `_lineRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that stores the line segment for tip based movement rather than projected mode. |
| `_lineSegment` | **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The mesh being used for the line visual to the interacting tool tip. |
| `_snapHighlight` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot storing the gizmo snap highlight visual. |
| `VectorSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space to do edits to the vector in. |
| `TargetVector` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >>** | The target vector field to modify. |
| `TargetRotation` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >>** | The target vector rotation to modify. |
| `FixMagnitude` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to fix a magnitude during/after editing. |
| `FixedMagnitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The value to fix the vector magnitude to if `FixMagnitude` is enabled. |
| `VisualMagnitudeScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The magnitude scalar of the vector visual. |
| `VisualThickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of the visual for the vector. |
| `_colliderRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the visual collider. |
| `_collider` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[CylinderCollider](https://wiki.resonite.com/Component:CylinderCollider "Component:CylinderCollider")** | The collider used for the vector. |
| `_mesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[ArrowMesh](https://wiki.resonite.com/Component:ArrowMesh "Component:ArrowMesh")** | The arrow mesh being used to show the vector visual. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VectorGizmo&oldid=106620](https://wiki.resonite.com/index.php?title=Component:VectorGizmo&oldid=106620)"

Contents