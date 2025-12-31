# Component:AvatarEyeTrackingInfo

> Source: https://wiki.resonite.com/Component:AvatarEyeTrackingInfo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarEyeTrackingInfo&diff=93716) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/21/AvatarEyeTrackingInfoComponent.png/510px-AvatarEyeTrackingInfoComponent.png)](https://wiki.resonite.com/File:AvatarEyeTrackingInfoComponent.png) **AvatarEyeTrackingInfo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarEyeTrackingInfo** is used to override the assigning behavior from a [Component:AvatarEyeDataSourceAssigner](https://wiki.resonite.com/Component:AvatarEyeDataSourceAssigner "Component:AvatarEyeDataSourceAssigner") on the avatar when it assigns a target.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `EyeDataSource` | **[IEyeDataSourceComponent](https://wiki.resonite.com/Type:IEyeDataSourceComponent "Type:IEyeDataSourceComponent")** | The data source to override the assigning behavior of a [Component:AvatarEyeDataSourceAssigner](https://wiki.resonite.com/Component:AvatarEyeDataSourceAssigner "Component:AvatarEyeDataSourceAssigner") on the avatar with. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarEyeTrackingInfo&oldid=93716](https://wiki.resonite.com/index.php?title=Component:AvatarEyeTrackingInfo&oldid=93716)"

Contents