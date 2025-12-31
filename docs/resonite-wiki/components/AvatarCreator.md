# Component:AvatarCreator

> Source: https://wiki.resonite.com/Component:AvatarCreator

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarCreator&diff=98329) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/eb/AvatarCreatorComponent.png/510px-AvatarCreatorComponent.png)](https://wiki.resonite.com/File:AvatarCreatorComponent.png) **Avatar Creator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The avatar creator component is the component that drives the functionality of the avatar creator object. See [Avatar Creation](https://wiki.resonite.com/Avatar_Creation "Avatar Creation") for a much less technical page on this, and for information on how to actually use the avatar creator.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_headsetPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the headset point that marks the head proxy target slot position. |
| `_leftPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the point that marks the left hand's target slot position. |
| `_rightPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the point that marks the right hand's target slot position. |
| `_leftFootPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the point that marks the foot's target slot position. |
| `_rightFootPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the point that marks the right foot target slot position. |
| `_pelvisPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the pelvis guide object that marks the pelvis proxy position. |
| `_headsetReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the headset guide that marks the headset proxy position (eyeballs/view position) |
| `_pelvisReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the pelvis guide object that marks the pelvis proxy position. |
| `_leftReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the left hand guide object that marks the left hand proxy. |
| `_rightReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the right hand guide object that marks the right hand proxy. |
| `_leftFootReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the left foot guide object. |
| `_rightFootReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the right foot guide object. |
| `_initialized` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether this avatar creator is ready to be used. |
| `_showAnchors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to show the tool anchors on the hands. |
| `_useSymmetry` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to enforce symmetry of the objects across the headset location during settup. |
| `_setupVolumeMeter` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set up a volume meter component on the avatar when the avatar is created. |
| `_setupProtection` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set up avatar protection components on the root and meshes of the avatar upon creation. |
| `_setupEyes` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set up the eye bones and [eye manager](https://wiki.resonite.com/Component:EyeManager "Component:EyeManager") upon avatar creation |
| `_setupFaceTracking` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set up a [face tracking component](https://wiki.resonite.com/Component:AvatarExpressionDriver "Component:AvatarExpressionDriver") for the mesh with the most shapekey matches for visemes. |
| `_calibrateFeet` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the feet calibration guide objects. |
| `_calibratePelvis` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to show the pelvis calibration guide object. |
| `_canProtect` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user is allowed to protect. This is false if in local. |
| `_symmetrySetup` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to enforce symmetry on the avatar when creating. |
| `_anchors` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AvatarCreator.Anchor](https://wiki.resonite.com/Component:AvatarCreator#Anchor)** | A list of [Anchor](https://wiki.resonite.com/Component:AvatarCreator#Anchor) that are the different parts for avatar markers the user can move when using this creator. |
| `_scale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the scale of all the `_anchors` of this avatar creator. |
| `_protectAvatarEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The protect avatar checkbox button enabled field. The checkbox disables when in user space |
| `_createEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field that controls the enabled state of the create avatar button. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnCreate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Avatar Creation](https://wiki.resonite.com/Avatar_Creation "Avatar Creation"). |
| `AlignHands:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Avatar Creation](https://wiki.resonite.com/Avatar_Creation "Avatar Creation"). |
| `AlignHeadPosition:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Avatar Creation](https://wiki.resonite.com/Avatar_Creation "Avatar Creation"). |
| `AlignHeadForward:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Avatar Creation](https://wiki.resonite.com/Avatar_Creation "Avatar Creation"). |
| `AlignHeadUp:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Avatar Creation](https://wiki.resonite.com/Avatar_Creation "Avatar Creation"). |
| `AlignHeadRight:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Avatar Creation](https://wiki.resonite.com/Avatar_Creation "Avatar Creation"). |
| `AlignToolAnchors:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Avatar Creation](https://wiki.resonite.com/Avatar_Creation "Avatar Creation"). |

Triggers
Collapse

## Anchor

| Name | Type | Description |
| --- | --- | --- |
| `ScaleDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of this guide object. |
| `AnchorName` | **[string](https://wiki.resonite.com/Type:String "Type:String")** | The human readable name of this guide object. |
| `IsRight` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this guide object is on the right side of the headset. (So is it a right or left hand for example?) |
| `Slot` | **[slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of this guide object. |
| `Slider` | [Slider](https://wiki.resonite.com/Component:Slider "Component:Slider") | The slider that can be used to move this guide object around via grabbing. |

Fields

## Usage

Used for creating avatars. You can spawn it from your Local Space if you have the Builder [Role](https://wiki.resonite.com/Roles_(Slot) "Roles (Slot)") permission to spawn it.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarCreator&oldid=98329](https://wiki.resonite.com/index.php?title=Component:AvatarCreator&oldid=98329)"

Contents