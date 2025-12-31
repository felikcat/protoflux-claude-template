# Component:MaterialRelay

> Source: https://wiki.resonite.com/Component:MaterialRelay

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MaterialRelay&diff=98525) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4f/MaterialRelayComponent.png/510px-MaterialRelayComponent.png)](https://wiki.resonite.com/File:MaterialRelayComponent.png) **Material Relay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MaterialRelay** component is used to specify to a [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool") when hitting a [slot](https://wiki.resonite.com/Slot "Slot") [tagged](https://wiki.resonite.com/Tag "Tag") with this component what materials to grab/apply to when using the tool.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MaterialRefs` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [Material](https://wiki.resonite.com/Type:Material "Type:Material") >** | A list of material storage fields that a material tool when applying should apply to. The first non null item in the list is the one a material tool will pick up when using the secondary action. |

Fields
Collapse

## Usage

Attach to the root of an object and provide a list of material storage fields from, for example, [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") or [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") to make Relays for.

## Examples

Added to the root of new avatars made with the avatar creator.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MaterialRelay&oldid=98525](https://wiki.resonite.com/index.php?title=Component:MaterialRelay&oldid=98525)"

Contents