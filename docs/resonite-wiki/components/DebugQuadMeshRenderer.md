# Component:DebugQuadMeshRenderer

> Source: https://wiki.resonite.com/Component:DebugQuadMeshRenderer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8c/DebugQuadMeshRendererComponent.png/510px-DebugQuadMeshRendererComponent.png)](https://wiki.resonite.com/File:DebugQuadMeshRendererComponent.png) **Debug Quad Mesh Renderer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugQuadMeshRenderer** component renders particles via a [Component:QuadArrayMesh](https://wiki.resonite.com/Component:QuadArrayMesh "Component:QuadArrayMesh").

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to use for the mesh. |

Fields
Collapse

## Usage

Attach to a slot, add to the renderer slot in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugQuadMeshRenderer&oldid=96379](https://wiki.resonite.com/index.php?title=Component:DebugQuadMeshRenderer&oldid=96379)"

Contents