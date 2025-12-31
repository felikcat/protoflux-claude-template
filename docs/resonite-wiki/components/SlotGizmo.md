# Component:SlotGizmo

> Source: https://wiki.resonite.com/Component:SlotGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0a/SlotGizmoComponent.png/510px-SlotGizmoComponent.png)](https://wiki.resonite.com/File:SlotGizmoComponent.png) **Slot Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SlotGizmo** is used with the [Dev tool](https://wiki.resonite.com/Dev_tool "Dev tool") to interact with slots when they are selected and their sub gizmos. This is rarely interacted directly with by the user, but is a very important component for interacting with the game.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `GizmoReplaced` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[SlotGizmo.SlotGizmoReplacement](https://wiki.resonite.com/Component:SlotGizmo#SlotGizmoReplacement)** | A sync delegate to call when the gizmo is replaced with another one. Usually located on the dev tool that created the gizmo. |
| `_isFolded` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the gizmo is folded up. |
| `_activeGizmo` | **[Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)")** | Which gizmo is being shown right now via tool options. |
| `_targetSlot` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The slot this is affecting. |
| `_positionDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive position with for this visual. |
| `_scaleDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive scale with for this visual. |
| `_boundsMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[TubeBoxMesh](https://wiki.resonite.com/Component:TubeBoxMesh "Component:TubeBoxMesh")** | The mesh to use to show bounds. |
| `_boundsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to make bounds for. |
| `_boundsRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | the field to drive for the bounds rotation. |
| `_boundsOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive for bounds offset. |
| `_boundsActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether the bounds are active or not. |
| `_nameText` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to drive with the name of the target slot. |
| `_nameOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position offset field for the visual of the name of targeted slot. |
| `_nameRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field for the visual of the name of targeted slot. |
| `_nameActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The active field for the visual of the name of targeted slot. |
| `_xPosSegment` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The segment used for the X position vs this slot's parent slot. |
| `_yPosSegment` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The segment used for the Y position vs this slot's parent slot. |
| `_zPosSegment` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The segment used for the Z position vs this slot's parent slot. |
| `_boundsAnchorPositions` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[SlotGizmo.AnchorInfo](https://wiki.resonite.com/Component:SlotGizmo#AnchorInfo)** | A list of infos for anchors this slot gizmo has. |
| `_rootAnchor` | **[PointAnchor](https://wiki.resonite.com/Component:PointAnchor "Component:PointAnchor")** | The root point anchor for this gizmo. |
| `_translationGizmo` | **[TranslationGizmo](https://wiki.resonite.com/Component:TranslationGizmo "Component:TranslationGizmo")** | The gizmo used for changing this slot's position. |
| `_rotationGizmo` | **[RotationGizmo](https://wiki.resonite.com/Component:RotationGizmo "Component:RotationGizmo")** | The gizmo used for changing this slot's rotation. |
| `_scaleGizmo` | **[ScaleGizmo](https://wiki.resonite.com/Component:ScaleGizmo "Component:ScaleGizmo")** | The gizmo used for changing this slot's scale. |
| `IsLocalSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this gizmo is oriented to local space or not. |

Fields
Collapse

## SlotGizmoReplacement

[Sync Delegate](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") of identity [Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") <SlotGizmo, SlotGizmo\> for replacing the old gimzo (argument 1) with a new one.

## AnchorInfo

| Name | Type | Description |
| --- | --- | --- |
| `anchor` | **[PointAnchor](https://wiki.resonite.com/Component:PointAnchor "Component:PointAnchor")** | The point anchor to snap to for other gizmos. |
| `posDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position to drive for this point anchor. |
| `scaleDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale to drive for this point anchor. |

Fields

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SlotGizmo&oldid=106566](https://wiki.resonite.com/index.php?title=Component:SlotGizmo&oldid=106566)"

Contents