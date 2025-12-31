# Component:AvatarMouthTrackingInfo

> Source: https://wiki.resonite.com/Component:AvatarMouthTrackingInfo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarMouthTrackingInfo&diff=93717) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/cf/AvatarMouthTrackingInfoComponent.png/510px-AvatarMouthTrackingInfoComponent.png)](https://wiki.resonite.com/File:AvatarMouthTrackingInfoComponent.png) **AvatarMouthTrackingInfo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarMouthTrackingInfo** is used to override the assigning behavior from a [Component:AvatarMouthDataSourceAssigner](https://wiki.resonite.com/Component:AvatarMouthDataSourceAssigner "Component:AvatarMouthDataSourceAssigner") on the avatar when it assigns a target. or when a [Component:AvatarExpressionDriver](https://wiki.resonite.com/Component:AvatarExpressionDriver "Component:AvatarExpressionDriver") on the avatar assigns it's own mouth data source.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MouthDataSource` | **[IMouthTrackingSourceComponent](https://wiki.resonite.com/Type:IMouthTrackingSourceComponent "Type:IMouthTrackingSourceComponent")** | The data source to override the assigning behavior of a [Component:AvatarMouthDataSourceAssigner](https://wiki.resonite.com/Component:AvatarMouthDataSourceAssigner "Component:AvatarMouthDataSourceAssigner") on the avatar with. or to override what a [Component:AvatarExpressionDriver](https://wiki.resonite.com/Component:AvatarExpressionDriver "Component:AvatarExpressionDriver") on the avatar assigns it's own mouth data source with. |

Fields
Collapse

## Usage

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarMouthTrackingInfo&oldid=93717](https://wiki.resonite.com/index.php?title=Component:AvatarMouthTrackingInfo&oldid=93717)"

Contents