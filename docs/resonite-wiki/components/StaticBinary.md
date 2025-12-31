# Component:StaticBinary

> Source: https://wiki.resonite.com/Component:StaticBinary

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:StaticBinary&diff=91576) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b6/StaticBinaryComponent.png/510px-StaticBinaryComponent.png)](https://wiki.resonite.com/File:StaticBinaryComponent.png) **Static Binary** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **StaticBinary** component is used to take in a [URL](https://wiki.resonite.com/Type:Uri "Type:Uri") and treats it like a [Binary](https://wiki.resonite.com/Type:Binary "Type:Binary") type, mostly used by other components.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The url to point to as being a binary for this component. |

Fields
Collapse

## Usage

This component can be combined with the [BinaryExportable](https://wiki.resonite.com/Component:BinaryExportable "Component:BinaryExportable") component to allow for exporting the [Slot](https://wiki.resonite.com/Slot "Slot") as a binary file on your device.

## Examples

This component can be combined with the [FileMetadata](https://wiki.resonite.com/Component:FileMetadata "Component:FileMetadata") component as part of how [Cloud Spawning](https://wiki.resonite.com/Cloud_Spawning "Cloud Spawning") works.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StaticBinary&oldid=91576](https://wiki.resonite.com/index.php?title=Component:StaticBinary&oldid=91576)"

Contents