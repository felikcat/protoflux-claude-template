# Component:AvatarEyeDataSourceAssigner

> Source: https://wiki.resonite.com/Component:AvatarEyeDataSourceAssigner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarEyeDataSourceAssigner&diff=93712) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ac/AvatarEyeDataSourceAssignerComponent.png/510px-AvatarEyeDataSourceAssignerComponent.png)](https://wiki.resonite.com/File:AvatarEyeDataSourceAssignerComponent.png) **Avatar Eye Data Source Assigner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarEyeDataSourceAssigner** component manages assigning eye tracking sources to fields

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetReference` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [IEyeDataSourceComponent](https://wiki.resonite.com/Type:IEyeDataSourceComponent "Type:IEyeDataSourceComponent") >** | The field to assign an eye tracking source to, unless it finds a [Component:AvatarEyeTrackingInfo](https://wiki.resonite.com/Component:AvatarEyeTrackingInfo "Component:AvatarEyeTrackingInfo") first, it assigns from that instead of the user's one. |

Fields
Collapse

## Usage

is used to assign the eye tracker for an avatar to a field when a user with eye tracking equips the avatar.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarEyeDataSourceAssigner&oldid=93712](https://wiki.resonite.com/index.php?title=Component:AvatarEyeDataSourceAssigner&oldid=93712)"

Contents