# Component:LocalMeshProvider

> Source: https://wiki.resonite.com/Component:LocalMeshProvider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/06/LocalMeshProviderComponent.png/510px-LocalMeshProviderComponent.png)](https://wiki.resonite.com/File:LocalMeshProviderComponent.png) **Local Mesh Provider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Local Mesh Provider** is a component that provides a local mesh. This is used internally to render things like UIX and particles.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |

Fields
Collapse

## Usage

Not used directly by the user.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocalMeshProvider&oldid=100874](https://wiki.resonite.com/index.php?title=Component:LocalMeshProvider&oldid=100874)"

Contents