# Component:VolumeTranslationGizmo

> Source: https://wiki.resonite.com/Component:VolumeTranslationGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8f/VolumeTranslationGizmoComponent.png/510px-VolumeTranslationGizmoComponent.png)](https://wiki.resonite.com/File:VolumeTranslationGizmoComponent.png) **Volume Translation Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VolumeTranslationGizmo** component is used to move around and edit a volume object.

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
| `PointSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space that the translation point is in. |
| `TargetPoint` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >>** | The field in which to drive for the target point editing. |
| `UseCustomVisual` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to use a custom visual. |
| `_customVisualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the custom visual element. |
| `_visualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the default visual. |
| `CubeSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size of the visual root. |
| `CreateUndoSteps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to create [Undo](https://wiki.resonite.com/Undo "Undo") steps for this gizmo. |
| `_cubeSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the cube size. |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the collider size. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VolumeTranslationGizmo&oldid=106622](https://wiki.resonite.com/index.php?title=Component:VolumeTranslationGizmo&oldid=106622)"

Contents