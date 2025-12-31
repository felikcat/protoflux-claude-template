# Component:AssetProxy

> Source: https://wiki.resonite.com/Component:AssetProxy

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AssetProxy&diff=93379) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/09/AssetProxy%601Component.png/510px-AssetProxy%601Component.png)](https://wiki.resonite.com/File:AssetProxy%601Component.png) **Asset Proxy\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Asset Proxy is a component that allows for access to an asset through a slot when being grabbed by the user.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AssetReference` | **A** | The asset to expose to asset ref fields when grabbing the object root of the slot this component is on. |

Fields
Collapse

## Usage

put this component on a slot and fill the `AssetReference` with an asset reference to allow access to an asset via holding this slot's object root. The asset will then be available when holding onto the object root of the slot this component is on, and clicking on a UIX field (ex: an inspector field) places the asset type that this component has inside of it into the field.

## Examples

This is used on items like imported audio clips and images, to allow them to be used and dropped into inspector fields.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AssetProxy&oldid=93379](https://wiki.resonite.com/index.php?title=Component:AssetProxy&oldid=93379)"

Contents