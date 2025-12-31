# Component:WorldLink

> Source: https://wiki.resonite.com/Component:WorldLink

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:WorldLink&diff=98211) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/22/WorldLinkComponent.png/510px-WorldLinkComponent.png)](https://wiki.resonite.com/File:WorldLinkComponent.png) **WorldLink** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldLink** component is used to set the [world](https://wiki.resonite.com/World "World") information, either to use as a way to jump to different worlds or to pre-load worlds.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The world to link. |
| `ActiveSessionURLs` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri") >** | Used for session orbs. |
| `CreateIfNotExists` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[WorldCreator](https://wiki.resonite.com/index.php?title=Type:WorldCreator&action=edit&redlink=1 "Type:WorldCreator (page does not exist)")** | If the world we are going to does not exist, then make one. |
| `WorldRelation` | **[Userspace.WorldRelation](https://wiki.resonite.com/Component:Userspace#WorldRelation "Component:Userspace")** | The relation of the world. |
| `AutoFocus` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | After the world loads, focus to this world automatically. |
| `GetExisting` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If a world we are looking for already exists, then don't make a new one and then optionally focus onto it. |

Fields
Collapse

## Usage

- This can be combined with the [ButtonWorldLink](https://wiki.resonite.com/Component:ButtonWorldLink "Component:ButtonWorldLink") component to setup a button for loading a world for a user.
- This can be hooked up into [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") with the [Open World](https://wiki.resonite.com/ProtoFlux:Open_World "ProtoFlux:Open World") or [Focus World](https://wiki.resonite.com/ProtoFlux:Focus_World "ProtoFlux:Focus World") nodes to open or jump to another world.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldLink&oldid=98211](https://wiki.resonite.com/index.php?title=Component:WorldLink&oldid=98211)"

Contents