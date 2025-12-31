# Component:AvatarMouthDataSourceAssigner

> Source: https://wiki.resonite.com/Component:AvatarMouthDataSourceAssigner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarMouthDataSourceAssigner&diff=91174) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/63/AvatarMouthDataSourceAssignerComponent.png/510px-AvatarMouthDataSourceAssignerComponent.png)](https://wiki.resonite.com/File:AvatarMouthDataSourceAssignerComponent.png) **AvatarMouthDataSourceAssigner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Avatar Mouth Data Source Assigner is a component that is able to assign a mouth tracking source to a field that accepts it.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetReference` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [IMouthTrackingSourceComponent](https://wiki.resonite.com/Type:IMouthTrackingSourceComponent "Type:IMouthTrackingSourceComponent") >** | A field that accepts a mouth tracking source (like `DataSource` on the [Avatar Expression Driver Component](https://wiki.resonite.com/Component:AvatarExpressionDriver "Component:AvatarExpressionDriver")) to assign a tracking source to. |

Fields
Collapse

## Behavior

This component is triggered when a user equips an avatar that has this component as part of the hierarchy. The user that equipped the avatar needs to have an active mouth data source on their client, such as a Vive facial tracker, or using a [mod](https://wiki.resonite.com/Mods "Mods") that creates a source for mouth tracking (like [VRCFTReceiver](https://github.com/hazre/VRCFTReceiver))

## Examples

This can be used to assign the mouth tracking source on a [Avatar Expression Driver Component](https://wiki.resonite.com/Component:AvatarExpressionDriver "Component:AvatarExpressionDriver") to enable facial movements on an avatar via facial tracking.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarMouthDataSourceAssigner&oldid=91174](https://wiki.resonite.com/index.php?title=Component:AvatarMouthDataSourceAssigner&oldid=91174)"

Contents