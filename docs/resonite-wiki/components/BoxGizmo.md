# Component:BoxGizmo

> Source: https://wiki.resonite.com/Component:BoxGizmo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BoxGizmo&diff=96232) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9b/BoxGizmoComponent.png/510px-BoxGizmoComponent.png)](https://wiki.resonite.com/File:BoxGizmoComponent.png) **Box Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BoxGizmo** component is used to make the handles and visual for editing a box mesh or collider, and also handles the interaction with the handles.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot of the box to edit. |
| `BoxCenterSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space to transform by when making the result of `BoxCenter` |
| `BoxSizeSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space to transform by when making the result of `BoxSize` |
| `BoxSize` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >>** | The field to edit for the box size. |
| `BoxCenter` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >>** | The field to drive for the box center. |
| `LockOffset` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to lock the offset of the box so it's center stays the same. |
| `_vertices` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | A list of fields to drive for the vertex positions of the cube gizmo visual. |
| `_edges` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | A list of fields to drive for the edge positions of the cube gizmo visual. |
| `_faces` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | A list of fields to drive for the face positions of the cube gizmo visual. |
| `_sphereColliderRadii` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | A list of fields to drive for the sphere rotations of the cube gizmo visual. |
| `_material` | **[OverlayFresnelMaterial](https://wiki.resonite.com/OverlayFresnelMaterial "OverlayFresnelMaterial")** | The material being used for the gizmo visual. |
| `_handleSphere` | **[IcoSphereMesh](https://wiki.resonite.com/Component:IcoSphereMesh "Component:IcoSphereMesh")** | The mesh being used for the handles of the gizmo like corners or faces. |
| `_visualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot of the visual root. |
| `_visualPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the visual position. |
| `_visualRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive for the visual rotation. |
| `_visualScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for the visual scale. |
| `_tubeBox` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[TubeBoxMesh](https://wiki.resonite.com/Component:TubeBoxMesh "Component:TubeBoxMesh")** | The tube box mesh being used for the gizmo visual. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used to edit box colliders or box meshes. Created by the dev tool when switching gizmo modes when having a box selected.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxGizmo&oldid=96232](https://wiki.resonite.com/index.php?title=Component:BoxGizmo&oldid=96232)"

Contents