# Component:SphereGizmo

> Source: https://wiki.resonite.com/Component:SphereGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2a/SphereGizmoComponent.png/510px-SphereGizmoComponent.png)](https://wiki.resonite.com/File:SphereGizmoComponent.png) **Sphere Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SphereGizmo** component is used to control the radius of certain sphere elements.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetSlot` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The slot this should position at. |
| `AutoPositionAtTargetSlot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether the gizmo should auto position at `TargetSlot` |
| `_interactingComponent` | **[Component](https://wiki.resonite.com/Type:Component "Type:Component")** | the tool interacting with this component. |
| `_material` | **[OverlayFresnelMaterial](https://wiki.resonite.com/OverlayFresnelMaterial "OverlayFresnelMaterial")** | The material that is being used for the visual. |
| `_toolPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The tool tip that is interacting with. |
| `_activePoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The active point slot for reference to an interacting tool. |
| `_lineRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The line root from this gizmo to a tool tip. |
| `_lineSegment` | **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The line mesh from this gizmo to a tool tip. |
| `_snapHighlight` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot used for highlighting snap targets. |
| `TargetRadius` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >>** | The field this gizmo is editing (also known as the radius field) |
| `RadiusSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The transform space the radius is in. |
| `RimRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the rim of the target radius. |
| `RimRadiusDistanceScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How to scale the radius for the rim by distance. |
| `_handles` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[SphereGizmo.Handle](https://wiki.resonite.com/Component:SphereGizmo#Handle)** | a list of handles for this gizmo. usually a set of 3 rings. |

Fields
Collapse

## Handle

| Name | Type | Description |
| --- | --- | --- |
| `RelativeRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The relative radius between the gizmo and this mesh. |
| `root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of this handle visual. |
| `mesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[TorusMesh](https://wiki.resonite.com/Component:TorusMesh "Component:TorusMesh")** | The torus mesh used for this visual. |

Fields

## Usage

Not used directly by the user. May have been one of the first components [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius") ever made for the game, considering that it doesn't follow some naming conventions that are never broken across all components, especially [SphereGizmo.Handle](https://wiki.resonite.com/Component:SphereGizmo#Handle) on this page.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SphereGizmo&oldid=106577](https://wiki.resonite.com/index.php?title=Component:SphereGizmo&oldid=106577)"

Contents