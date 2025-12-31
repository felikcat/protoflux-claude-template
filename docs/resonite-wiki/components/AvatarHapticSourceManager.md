# Component:AvatarHapticSourceManager

> Source: https://wiki.resonite.com/Component:AvatarHapticSourceManager

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b8/AvatarHapticSourceManagerComponent.png/510px-AvatarHapticSourceManagerComponent.png)](https://wiki.resonite.com/File:AvatarHapticSourceManagerComponent.png) **Avatar Haptic Source Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarHapticSourceManager** component allows you to override the injected haptic points that Resonite puts on fullbody avatars and to specify custom [Haptic Volumes](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") on your body.

Overriding your injected haptic points can be useful in situations where your avatar's proportions exaggerate the automatic haptic points that other users feel is too large or too small.

Requires the avatar to be equipped again to turn off the injected haptics.

Despite the component asking for the [haptic volume](https://wiki.resonite.com/Component:HapticVolume "Component:HapticVolume") active state, it is suggested to instead use the active state of the haptic [collider](https://wiki.resonite.com/Collider "Collider"), this allows the Avatar Haptic Source Manager to disable the colliders on the active user and allow culling behavior. The reason for this is that disabling haptic volumes does not disable the haptics itself.

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HapticVolumeActiveStates` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Drives the boolean field put in the list to be disabled when noclipping usually |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

While Avatar Haptic Source Manger controls overriding the haptic volumes on your avatar, [Controller Haptic Point Mapper](https://wiki.resonite.com/Component:ControllerHapticPointMapper "Component:ControllerHapticPointMapper") controls where you receive haptic events on your controllers.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarHapticSourceManager&oldid=97239](https://wiki.resonite.com/index.php?title=Component:AvatarHapticSourceManager&oldid=97239)"

Contents