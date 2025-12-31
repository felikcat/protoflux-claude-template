# Component:MeshRendererLoadStatus

> Source: https://wiki.resonite.com/Component:MeshRendererLoadStatus

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MeshRendererLoadStatus&diff=94871) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8f/MeshRendererLoadStatusComponent.png/510px-MeshRendererLoadStatusComponent.png)](https://wiki.resonite.com/File:MeshRendererLoadStatusComponent.png) **Mesh Renderer Load Status** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MeshRendererLoadStatus** component keeps track of how many meshes in the list of meshes have been loaded for the local user. The meshes can be skinned mesh renderers or mesh renderers. The loaded status checks for if the mesh is loaded, including for any materials on those mesh/skinned mesh renderers.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Renderers` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | A list of skinned mesh renderers or mesh renderers to keep track of the load progress for. |
| `IsLoaded` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether all meshes are finished loading |
| `LoadProgress` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The percentage of meshes that have loaded. |
| `ProgressWeight` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The number of not null meshes that exist in `Renderers`. |

Fields
Collapse

## Usage

Can be used for a loading indicator for worlds or avatars.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:UsersAssetLoadProgress](https://wiki.resonite.com/Component:UsersAssetLoadProgress "Component:UsersAssetLoadProgress")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshRendererLoadStatus&oldid=94871](https://wiki.resonite.com/index.php?title=Component:MeshRendererLoadStatus&oldid=94871)"

Contents