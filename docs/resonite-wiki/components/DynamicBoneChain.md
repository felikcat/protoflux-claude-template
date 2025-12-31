# Component:DynamicBoneChain

> Source: https://wiki.resonite.com/Component:DynamicBoneChain

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5b/DynamicBoneChainComponent.png/510px-DynamicBoneChainComponent.png)](https://wiki.resonite.com/File:DynamicBoneChainComponent.png) **Dynamic Bone Chain** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Dynamic Bone Chain is a component that allows you to add [rigidbody](https://en.wikipedia.org/wiki/Rigid_body) physics to the bones of a rigged model or avatar. Bones with rigidbody physics are called dynamic bones; this name is derived from a [Unity asset](https://assetstore.unity.com/packages/tools/animation/dynamic-bone-16743) that offers similar functionality.

To add dynamic bones to a model, navigate through the model's armature in the Inspector until you locate the bone you want to use as the "root" or "master" bone. Then, attach the Dynamic Bone Chain component, and click Setup From Children. This will add the root bone and all its children to the dynamic bone chain.

The Dynamic Bone Chain component contains various properties for adjusting the physical behavior of the bone chain. The most important properties in the component are Inertia, InertiaForce, Damping, Elasticity, and Stiffness. The descriptions of each are listed below:

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Inertia` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls the amount of inertia a bone experiences. Does not affect acceleration of bones. |
| `InertiaForce` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls the amount of inertia a bone experiences. Does affect acceleration of bones. |
| `Damping` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls the amount of damping a bone experiences. A high damping value will cause bones to decelerate quickly. |
| `Elasticity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls the elasticity of bone joints. A high elasticity value will cause bones to accelerate toward their starting rotation more quickly. |
| `Stiffness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls the stiffness of bone joints. |
| `SimulateTerminalBones` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to use the last bone in the chain. If your armature has end bones that do not control anything, you probably want this off. |
| `BaseBoneRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The default size of the sphere that allows a bone to be interacted with. |
| `DynamicPlayerCollision` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow this bone chain to collide with players. |
| `CollideWithOwnBody` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow this bone chain to collide with the active user of the dynamic bone chain. |
| `HandCollisionVibration` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | The vibration intensity when touching the chain colliders with a hand. |
| `CollideWithHead` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow this bone chain to collide with player heads. |
| `CollideWithBody` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow this bone chain to collide with player body parts. |
| `CollideWithLeftHand` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow this bone chain to collide with a player's left hand. |
| `CollideWithRightHand` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow this bone chain to collide with a player's right hand. |
| `Gravity` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | A force like gravity in `GravitySpace` space that should be applied to the bone chain at all times. |
| `GravitySpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space to apply `Gravity` in. |
| `UseUserGravityDirection` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to use the active user of the dynamic bone chain's character controller gravity for the gravity direction |
| `LocalForce` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Constant force being applied to the bone in the dynamic bone chain's local space. |
| `GlobalStretch` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How stretched out the bone chain should be at rest. |
| `MaxStretchRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum amount of stretching that can be caused by pulling on the bones. |
| `CurrentStretchRatio` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current amount of stretching applied to the bones. |
| `StretchRestoreSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How quickly extra stretching dissipates. |
| `UseLocalUserSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to make the dynamic bone only respond to movements generated from the user slot's local position changing. |
| `SimulationSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space that movement in should affect this dynamic bone chain. |
| `StaticColliders` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IDynamicBoneCollider](https://wiki.resonite.com/Type:IDynamicBoneCollider "Type:IDynamicBoneCollider")** | A list of dynamic bone collider components to be used. |
| `VisualizeColliders` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Causes all bone colliders colliding with this bone to be displayed. |
| `VisualizeBones` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Causes the bones, their colliders, and the connections between them to be displayed. |
| `IsGrabbable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allows you to grab bones by touching them and grabbing. Requires DynamicPlayerCollision to be checked. |
| `ActiveUserRootOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allows the active user of the dynamic bone chain to be the only user that can grab it. |
| `AllowSteal` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not a second user can grab the chain while someone is holding it. |
| `GrabPriority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Determines what gets grabbed if several grabbable objects are touching someone's grab sphere. The [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") with the highest priority will be grabbed first. If the highest priority ties with another [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"), it will grab both of those and ignore any lower priority [IGrabbables](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"). |
| `IgnoreGrabOnFirstBone` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Prevents EffectorBoneIndex from being 0 while being grabbed. |
| `GrabRadiusTolerance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much further a user can grab a bone with their grab sphere despite the radius of the bone not being in contact with their grab sphere. |
| `GrabReleaseDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far a bone can be dragged before it automatically releases. |
| `GrabSlipping` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to make the EffectorBoneIndex increase as the hand moves along the bone chain away from the first bone in the chain. Does not let EffectorBoneIndex decrease unless re-grabbed. |
| `GrabTerminalBones` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the final bone in the chain can be grabbed. |
| `GrabVibration` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | The vibration intensity when grabbing the chain with a hand. |
| `IgnoreOwnLeftHand` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow this bone chain to be grabbed with the left hand of the active user of the dynamic bone chain. |
| `IgnoreOwnRightHand` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow this bone chain to be grabbed with the right hand of the active user of the dynamic bone chain. |
| `EffectorTarget` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The chain tries to position one if its bones at this slot (used for grabbing) |
| `EffectorBoneIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Which bone is being positioned, every other bone after this acts as if it is not being grabbed |
| `EffectorBoneOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | acts as an offset from the grabbing slot in the grabbing slot's local space at the moment the bone was grabbed. Essentially prevents the bone from snapping to the center of the hand's grab sphere and keeps an offset for a smoother grabbing experience. Is automatically set every grab. |
| `_activeGrabber` | **[Grabber](https://wiki.resonite.com/Component:Grabber "Component:Grabber")** | The grabber component that is grabbing this bone chain currently |
| `Bones` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[DynamicBoneChain.Bone](https://wiki.resonite.com/Component:DynamicBoneChain#Bone)** | The bones that should be controlled by this dynamic bone chain. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetupFromChildren:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Sets up bones from children, ignoring ones already driven. |
| `SetupFromAllChildren:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Sets up all children bones, regardless of if they are driven by breaking the drive links and replacing them with ones from this component. |
| `SetupFromAllRigChildren:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | sets up child bones as dynamic bones for this component. Ignores all slots except for one's epecified in a [Rig component](https://wiki.resonite.com/Component:Rig "Component:Rig") on a slot that is a parent to the slot this dynamic bone component is on. |
| `ReplaceSmoothTransforms:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Replace any smooth transforms affecting the bones targeted by this chain with drives from this chain. |
| `AddCollidersFromHierarchy:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Add all colliders in hiearchy under this bone that are dynamic bone colliders to this bone chain's `StaticColliders` list. |
| `AlwaysGrabLastBone:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | changes the `GrabOverride` on every [Bone](https://wiki.resonite.com/Component:DynamicBoneChain#Bone) in the chain to point to the last bone in the chain. |
| `CleanSmoothTransforms:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Gets rid of smooth transforms on targeted bones. |

Triggers
Collapse

## Bone

| Name | Type | Description |
| --- | --- | --- |
| `BoneSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot of the dynamic bone this bone is referring to. |
| `OrigPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The rest position of `BoneSlot`. |
| `OrigRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rest rotation of `BoneSlot`. |
| `RadiusModifier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to multiply the default radius specified by the dynamic bone chain to make this bone's radius. |
| `GrabOverride` | **[Bone](https://wiki.resonite.com/Component:DynamicBoneChain#Bone)** | A Bone the same type as this Bone that will be grabbed instead of this bone when this bone is grabbed. |
| `Collide` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this bone has collisions. |
| `_posDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of `BoneSlot` which this should be driving to make the dynamic bone movement effects. |
| `_rotDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation `BoneSlot` which this should be driving to make the dynamic bone movement effects. |

Fields

### Bone Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnSetupFromSlot():ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Sets up the `OrigPosition`, `OrigRotation`, `_rotDrive`, and `_posDrive` fields of the [Bone](https://wiki.resonite.com/Component:DynamicBoneChain#Bone) when pressed and `BoneSlot` is not null. |

Triggers
Collapse

## Usage

## Examples

[Community Presets](https://wiki.resonite.com/Dynamic_bone_chain_parameters "Dynamic bone chain parameters")

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicBoneChain&oldid=113866](https://wiki.resonite.com/index.php?title=Component:DynamicBoneChain&oldid=113866)"

Contents