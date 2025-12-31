# Component:DebugTangentSpace

> Source: https://wiki.resonite.com/Component:DebugTangentSpace

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2e/DebugTangentSpace.png/510px-DebugTangentSpace.png)](https://wiki.resonite.com/File:DebugTangentSpace.png) **Debug Tangent Space** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component was added in [Beta 2023.12.15.22](https://wiki.resonite.com/Beta_2023.12.15.22 "Beta 2023.12.15.22") to diagnose tangent space on meshes.

It may be removed at any time in the future.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Mesh` | **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | The mesh renderer to Debug tangents for. |
| `Triangle` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The triangle index to Debug tangents for. |
| `BaryCoord` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Used as an interpolator for the tangents and normals of the target triangle. |
| `RadiusRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | unused. |

Fields
Collapse

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugTangentSpace&oldid=96390](https://wiki.resonite.com/index.php?title=Component:DebugTangentSpace&oldid=96390)"

Contents