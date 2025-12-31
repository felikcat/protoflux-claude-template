# Component:AvatarControllerInfo

> Source: https://wiki.resonite.com/Component:AvatarControllerInfo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarControllerInfo&diff=91548) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fc/AvatarControllerInfoComponent.png/510px-AvatarControllerInfoComponent.png)](https://wiki.resonite.com/File:AvatarControllerInfoComponent.png) **AvatarControllerInfo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Reads the controller FrooxEngine class type and it's model identifier for a [User](https://wiki.resonite.com/Type:User "Type:User") for a hand [Side](https://wiki.resonite.com/Type:Chirality "Type:Chirality").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user this component is reading controller info from |
| `ControllerSide` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | The side (left or right) controller this component is reading info from. |
| `ControllerType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The type of the controller `TargetUser` is using on their `ControllerSide` hand. |
| `ControllerDeviceModel` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The device model of the controller `TargetUser` is using on their `ControllerSide` hand. |

Fields
Collapse

## Behavior

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarControllerInfo&oldid=91548](https://wiki.resonite.com/index.php?title=Component:AvatarControllerInfo&oldid=91548)"

Contents