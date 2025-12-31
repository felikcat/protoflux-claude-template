# Component:FileMetadata

> Source: https://wiki.resonite.com/Component:FileMetadata

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:FileMetadata&diff=98404) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ec/FileMetadataComponent.png/510px-FileMetadataComponent.png)](https://wiki.resonite.com/File:FileMetadataComponent.png) **File Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

File metadata is a component used in RawFile object imports and is often taken advantage of for [Cloud Spawning](https://wiki.resonite.com/Cloud_Spawning "Cloud Spawning").

This component has two [sync delegates](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") which import and export data from a [Static Binary Component](https://wiki.resonite.com/Component:StaticBinary "Component:StaticBinary") on the same slot.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Filename` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the file, usually followed by .brson or .7bson |
| `MIME` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | see [Media Types (MIME)](https://en.wikipedia.org/wiki/Media_type) |
| `IsProcessing` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether this component is currently processing an import or export action asynchronously. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnImportFile:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Cloud Spawning](https://wiki.resonite.com/Cloud_Spawning "Cloud Spawning"). |
| `OnExportFile:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | See [Cloud Spawning](https://wiki.resonite.com/Cloud_Spawning "Cloud Spawning"). |

Triggers
Collapse

## Usage

See [Cloud Spawning](https://wiki.resonite.com/Cloud_Spawning "Cloud Spawning").

## Examples

Usually used in RawFile object imports created by importing files from a local computer.

## Related Components

- [Static Binary](https://wiki.resonite.com/Component:StaticBinary "Component:StaticBinary")

## See Also

[Media Types (MIME)](https://en.wikipedia.org/wiki/Media_type)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FileMetadata&oldid=98404](https://wiki.resonite.com/index.php?title=Component:FileMetadata&oldid=98404)"

Contents