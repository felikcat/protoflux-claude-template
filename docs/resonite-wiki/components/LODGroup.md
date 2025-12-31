# Component:LODGroup

> Source: https://wiki.resonite.com/Component:LODGroup

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/33/LODGroupComponent.png/510px-LODGroupComponent.png)](https://wiki.resonite.com/File:LODGroupComponent.png) **LODGroup** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

A LOD (Level Of Detail) Group allows you to define behaviors to load alternate meshes for objects based on their relative size on a user's screen. This is commonly used to replace complex and finely detailed meshes with simplified versions based on a user's distance from the object.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LODs` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LODGroup.LOD](https://wiki.resonite.com/Component:LODGroup#LOD)** | A list of different LOD stages with renderers that should appear for each stage. |
| `CrossFade` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Cross fade on the Unity LOD component. |
| `AnimateCrossFading` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Animate Cross fade on the Unity LOD component. |

Fields
Collapse

## LOD

| Name | Type | Description |
| --- | --- | --- |
| `ScreenRelativeTransitionHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This defines the minimum size of the object to use this LOD stage. |
| `FadeTransitionWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | FadeTransitionWidth on the Unity LOD component. |
| `Renderers` | _direct_ **[SyncRelayList\`1](https://wiki.resonite.com/index.php?title=Type:SyncRelayList%601&action=edit&redlink=1 "Type:SyncRelayList`1 (page does not exist)") < [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") >** | List of mesh renderers that should belong to this component, which become Mesh Renderers from the UnityEngine when they are injected by [FrooxEngine](https://wiki.resonite.com/FrooxEngine "FrooxEngine") into the unity scene forcibly via it's rendering pipeline. |

Fields

## Behavior

This also influences the images seen of renderers viewed in mirrors. meaning that a renderer specified by this component can look different in the mirror vs if it's right beside you, at the exact same moment.

This component relies heavily on the behavior of Unity when it's forced to the unity side via Connectors in [FrooxEngine](https://wiki.resonite.com/FrooxEngine "FrooxEngine").

## Examples

A simple LODGroup would be specific stages where the object doesn't appear to lose any detail due to the smaller size.

[![](https://wiki.resonite.com/images/thumb/2/26/LOD_Example.png/300px-LOD_Example.png)](https://wiki.resonite.com/File:LOD_Example.png)

This example object will switch from the Sphere when the object is taking up 30% of the rendered screen, and to the cube when it's 5% of the rendered screen, and finally de-rendering entirely when it's smaller than that.

## See Also

- [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LODGroup&oldid=101145](https://wiki.resonite.com/index.php?title=Component:LODGroup&oldid=101145)"

Contents