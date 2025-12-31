# Component:MeshRendererMaterialRelay

> Source: https://wiki.resonite.com/Component:MeshRendererMaterialRelay

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7a/MeshRendererMaterialRelayComponent.png/510px-MeshRendererMaterialRelayComponent.png)](https://wiki.resonite.com/File:MeshRendererMaterialRelayComponent.png) **Mesh Renderer Material Relay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MeshRendererMaterialRelay** component relays the application of a [slot](https://wiki.resonite.com/Slot "Slot") [tagged](https://wiki.resonite.com/Tag "Tag") with this component [Material](https://wiki.resonite.com/Material "Material") applied by the [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool") to the the [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")'s in the Renderers list.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Renderers` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | The list of renderers to relay to the material tool. |
| `_renderer` | **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | An extra renderer that's legacy. |

Fields
Collapse

## Usage

Attach to a slot and provide the mesh renderers that should have materials applied to them with the material Tool in `Renderers`.

## Examples

This component is applied to an [Avatar](https://wiki.resonite.com/Avatar "Avatar") by default when created with the [Avatar Creator](https://wiki.resonite.com/Avatar_Creator "Avatar Creator").

## See Also

- [Material Tool](https://wiki.resonite.com/Material_Tool "Material Tool")
- [Component:MaterialRelay](https://wiki.resonite.com/Component:MaterialRelay "Component:MaterialRelay")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshRendererMaterialRelay&oldid=98526](https://wiki.resonite.com/index.php?title=Component:MeshRendererMaterialRelay&oldid=98526)"

Contents