# Component:PositionAtUser

> Source: https://wiki.resonite.com/Component:PositionAtUser

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PositionAtUser&diff=98204) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/52/PositionAtUserComponent.png/510px-PositionAtUserComponent.png)](https://wiki.resonite.com/File:PositionAtUserComponent.png) **PositionAtUser** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PositionAtUser** component drives the values in `PositionDrive` and `RotationDrive` to match the user's position and rotation as determined by the settings in `PositionSource` and `RotationSource` respectively.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that will be used to calculate the parent slot position, unless `PositionAtLocalUser` is selected. |
| `PositionAtLocalUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Position the parent slot at the [Local User](https://wiki.resonite.com/index.php?title=Local_User&action=edit&redlink=1 "Local User (page does not exist)") of each client, ignoring the value in `TargetUser` |
| `TargetPositionOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Position offset in the user's local space units. Respects the user's current scale and transforms. |
| `TargetRotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Rotation offset in the user's local space unit. Respects the user's current scale and transforms. |
| `PositionOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Position offset in global space units |
| `RotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Rotation offset in global space units |
| `PositionSource` | **[UserRoot.UserNode](https://wiki.resonite.com/Component:UserRoot#UserNode "Component:UserRoot")** | The user node that the position will be calculated from |
| `RotationSource` | **[UserRoot.UserNode](https://wiki.resonite.com/Component:UserRoot#UserNode "Component:UserRoot")** | The user node that the rotation will be calculated from |
| `PositionDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Target Float3 to drive with the calculated position value |
| `RotationDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Target FloatQ to drive with the calculated rotation value. |

Fields
Collapse

## Behavior

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PositionAtUser&oldid=98204](https://wiki.resonite.com/index.php?title=Component:PositionAtUser&oldid=98204)"

Contents