# Component:AvatarAnchor

> Source: https://wiki.resonite.com/Component:AvatarAnchor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f6/AvatarAnchorComponent.png/510px-AvatarAnchorComponent.png)](https://wiki.resonite.com/File:AvatarAnchorComponent.png) **AvatarAnchor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

An anchor allows for an [avatar](https://wiki.resonite.com/Avatar "Avatar") to be attached to a [slot](https://wiki.resonite.com/Slot "Slot"). This component can also allow for pinning of a user's limb(s) for posing, and is most commonly used as a seat.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Highlight` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether a user is pointing at this anchor and it is possible for them to activate the enter dialogue by pressing Primary at this moment. |
| `ParentSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space in which to work with the avatar. |
| `MinScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If an avatar has a scale below the MinScale, it will be scaled up to that size. |
| `MaxScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | If an avatar has a scale above the MaxScale, it will be scaled down to that size. |
| `PositionNode` | **[UserRoot.UserNode](https://wiki.resonite.com/Component:UserRoot#UserNode "Component:UserRoot")** | Which part of the avatar to use to position the avatar. |
| `PositionReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to position the avatar to. |
| `RotationNode` | **[UserRoot.UserNode](https://wiki.resonite.com/Component:UserRoot#UserNode "Component:UserRoot")** | Which part of the avatar to use to rotate the avatar. |
| `RotationReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to rotate the avatar to. |
| `PreserveUpOnEnter` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to keep the user's root slot's up direction pointing the same direction it was in global space before entering, or to align them to the up of the slot of the anchor. This is disabled when `RotationNode` and `RotationReference` are set to not none. |
| `PreserveUpOnExit` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to keep the user's root slot's up direction pointing the same direction it was in global space before exiting, or to align them to the up of the slot they get parented back under. This is disabled when `TransformRestoreMode` and `RestoreNode` are set to not none. |
| `UnparentEverythingOnDestroy` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Unparent all slots under `ParentSpace`'s Space slot and parent them under the parent of the nearest ObjectRoot (doesn't need an explicit ObjectRoot component). If `ParentSpace`'s Space slot is null, or the ObjectRoot parent is null, then all children are deleted anyway. |
| `TransformRestoreMode` | **[AvatarAnchor.RestoreMode](https://wiki.resonite.com/Component:AvatarAnchor#RestoreMode)** | What slot or space to use when setting the user's transforms to what they were before they entered the anchor. |
| `RestoreNode` | **[UserRoot.UserNode](https://wiki.resonite.com/Component:UserRoot#UserNode "Component:UserRoot")** | The part of the user's avatar that the transforms should be changed to `_originalPosition`, `_originalRotation`, and `_originalScale` when the user exits the anchor. Which space the transforms refer to (aka what it would be parented to) depends on what `TransformRestoreMode` is set to. |
| `RestoreReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | This will be used from when `TransformRestoreMode` is set to "Reference". The specified `RestoreNode`'s transform will be set to this slot's space using `_originalPosition`, `_originalRotation`, and `_originalScale`. |
| `Filters` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AvatarAnchor.BodyNodeFilters](https://wiki.resonite.com/Component:AvatarAnchor#BodyNodeFilters)** | A list of pose filters to use. Each one can control the position, rotation, and/or speed of a specific body node |
| `UserFilters` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IAvatarAnchorUserFilter](https://wiki.resonite.com/index.php?title=Type:IAvatarAnchorUserFilter&action=edit&redlink=1 "Type:IAvatarAnchorUserFilter (page does not exist)")** | Nothing currently implements [IAvatarAnchorUserFilter](https://wiki.resonite.com/index.php?title=Type:IAvatarAnchorUserFilter&action=edit&redlink=1 "Type:IAvatarAnchorUserFilter (page does not exist)") so this currently does nothing. |
| `UserAnchored` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[AvatarAnchorUserEvent](https://wiki.resonite.com/index.php?title=Type:AvatarAnchorUserEvent&action=edit&redlink=1 "Type:AvatarAnchorUserEvent (page does not exist)")** | Internal |
| `UserStay` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[AvatarAnchorUserEvent](https://wiki.resonite.com/index.php?title=Type:AvatarAnchorUserEvent&action=edit&redlink=1 "Type:AvatarAnchorUserEvent (page does not exist)")** | Internal |
| `UserReleased` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[AvatarAnchorUserEvent](https://wiki.resonite.com/index.php?title=Type:AvatarAnchorUserEvent&action=edit&redlink=1 "Type:AvatarAnchorUserEvent (page does not exist)")** | Internal |
| `_originalSpace` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Internal |
| `_originalPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Internal |
| `_originalRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Internal |
| `_originalScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Internal |
| `_dummyObjectSlots` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot")** | Internal |

Fields
Collapse

## BodyNodeFilters

| Name | Type | Description |
| --- | --- | --- |
| `Node` | **[BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")** | The node on the anchored user to apply filters to. |
| `Required` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether full body users can override this node and move the body part anyway. |
| `Filters` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[PoseFilter](https://wiki.resonite.com/Component:AvatarAnchor#PoseFilter)** | The list of filters that should be applied to `Node` when the user is anchored. |

Fields

## PoseFilter

| Name | Type | Description |
| --- | --- | --- |
| `Filter` | **[IAvatarPoseFilter](https://wiki.resonite.com/Type:IAvatarPoseFilter "Type:IAvatarPoseFilter")** | Any [Pose Filter](https://wiki.resonite.com/Category:Components:Users:Common_Avatar_System:Pose_Filters "Category:Components:Users:Common Avatar System:Pose Filters") can be used here to be applied to a body node. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Whether to apply the pose filter before another pose filter. |

Fields

## Behavior

By itself, an AvatarAnchor does nothing. It requires either an [AvatarAnchorTouchTrigger](https://wiki.resonite.com/AvatarAnchorTouchTrigger_(Component) "AvatarAnchorTouchTrigger (Component)") component or a [Anchor User](https://wiki.resonite.com/ProtoFlux:Anchor_User "ProtoFlux:Anchor User") [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") node to place an avatar into it.

To exit an anchor, a [AvatarAnchorLocomotionRelease](https://wiki.resonite.com/AvatarAnchorLocomotionRelease_(Component) "AvatarAnchorLocomotionRelease (Component)") component or a [Release User](https://wiki.resonite.com/ProtoFlux:Release_User "ProtoFlux:Release User") [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") node needs to be used.

When a user is anchored to an an anchor, first `TransformRestoreMode` takes it's effect on the settings (see above table for any field descriptions). Next the user root slot is parented under `ParentSpace`. Then `MinScale` and `MaxScale` are applied to keep the avatar within the right size. After that the global rotation and position of the user's root slot is set to the global position and rotation of the `PositionReference` and `RotationReference` slots using their specified nodes. Lastly the avatar's filters are applied.

## Examples

Chairs, cars, planes, etc.

## See Also

- [Component:MultiUserAvatarAnchor](https://wiki.resonite.com/Component:MultiUserAvatarAnchor "Component:MultiUserAvatarAnchor")
- [Component:GrabbableAvatarPoseFilter](https://wiki.resonite.com/Component:GrabbableAvatarPoseFilter "Component:GrabbableAvatarPoseFilter")
- Component:AvatarAnchor
- [Component:ToolAvatarPoseFilter](https://wiki.resonite.com/Component:ToolAvatarPoseFilter "Component:ToolAvatarPoseFilter")
- [Component:AvatarPoseOffset](https://wiki.resonite.com/Component:AvatarPoseOffset "Component:AvatarPoseOffset")
- [Component:AvatarPoseSmoothLerp](https://wiki.resonite.com/Component:AvatarPoseSmoothLerp "Component:AvatarPoseSmoothLerp")
- [Component:AvatarPoseRotationConstraint](https://wiki.resonite.com/Component:AvatarPoseRotationConstraint "Component:AvatarPoseRotationConstraint")
- [Component:AvatarPoseBoxConstraint](https://wiki.resonite.com/Component:AvatarPoseBoxConstraint "Component:AvatarPoseBoxConstraint")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarAnchor&oldid=101707](https://wiki.resonite.com/index.php?title=Component:AvatarAnchor&oldid=101707)"

Contents