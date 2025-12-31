# Component:HapticManager

> Source: https://wiki.resonite.com/Component:HapticManager

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/27/HapticManagerComponent.png/510px-HapticManagerComponent.png)](https://wiki.resonite.com/File:HapticManagerComponent.png) **Haptic Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This works as part of the game's robust [Haptics](https://wiki.resonite.com/Haptics "Haptics") system.

Can be found under each user's User root [slot](https://wiki.resonite.com/Slot "Slot"), the HapticManager controls the locally injected haptics for everyone in the session besides yourself if this component is found underneath your own user root slot.

The HapticManager also allows you to locally see the debug visuals of each user in the form of green transparent shapes. However you need to check ShowDebugVisuals then hit Rebuild Injected Sources to see this change reflected, do the inverse to remove the debug visuals.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `InjectedBodyPartIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Adjusts the haptic intensity of bodyparts that aren't the head and hands. |
| `InjectedHandIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Adjusts the haptic intensity of the hands. |
| `InjectedHeadIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Adjusts the haptic intensity of the head. |
| `InjectedRadiusStartRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Adjusts the start radius of all injected haptics. |
| `InjectedRadiusEndRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Adjusts the end radius of all injected haptics. |
| `InjectedRadiusPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Adjusts the overall radius of all injected haptics. |
| `ShowDebugVisuals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Locally shows injected haptics for each user, Rebuild Injected Sources needs to be checked for this to work. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnRebuild:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Recreates all the samplers on the user for haptic devices. |

Triggers
Collapse

## Usage

Note this component functions locally and does _not_ affect injected haptics on your own avatar, to do that you need to use the [AvatarHapticSourceManager](https://wiki.resonite.com/Component:AvatarHapticSourceManager "Component:AvatarHapticSourceManager") to override the injected behavior for your own avatar. If found on other user root slots other than yourself, this component does nothing and won't do any changes.

HapticManger can be used to debug weird haptic collisions from other users in the session, or possibly help with the issues where there is "stuck" haptics from touching injected haptic zones by rebuilding the haptic zones.

With the help of the ShowDebugVisuals you can see the haptic culling behavior if you step away from another user far enough.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HapticManager&oldid=98448](https://wiki.resonite.com/index.php?title=Component:HapticManager&oldid=98448)"

Contents