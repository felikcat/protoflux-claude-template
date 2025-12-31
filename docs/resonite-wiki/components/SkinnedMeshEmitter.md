# Component:SkinnedMeshEmitter

> Source: https://wiki.resonite.com/Component:SkinnedMeshEmitter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d6/SkinnedMeshEmitterComponent.png/510px-SkinnedMeshEmitterComponent.png)](https://wiki.resonite.com/File:SkinnedMeshEmitterComponent.png) **Skinned Mesh Emitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

A skinned mesh renderer can be used to emit particles from either the vertices, edges, or faces of a [SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer"). The colors of the particles can be made to be the colors of certain points of a texture, which is sampled via which point on the skinned mesh renderer the particle is emitted from.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `System` | **[ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")** | The particle system to get data from like style and particle count limits. |
| `Rate` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how fast to emit particles into the system. |
| `BurstOnActivatedMin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum value of the range of particle count to be emitted when activated as a burst. |
| `BurstOnActivatedMax` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum value of the range of particle count to be emitted when activated as a burst. |
| `BurstOnStart` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not particle bursts should be done on spawn. |
| `EmitFrom` | **[MeshEmissionSource](https://wiki.resonite.com/Type:MeshEmissionSource "Type:MeshEmissionSource")** | What parts of the mesh to emit from. |
| `UseVertexColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the vertex color data from the mesh for the color of the particles. |
| `DirectionMode` | **[MeshEmitterDirection](https://wiki.resonite.com/index.php?title=Type:MeshEmitterDirection&action=edit&redlink=1 "Type:MeshEmitterDirection (page does not exist)")** | the coordinate direction to use for up. |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Which direction in local space to shoot particles emitted by this emitter. |
| `RandomDirectionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to randomize the velocity of new particles (this is a magnitude) |
| `ColorTexture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to use as the colors of the emitted particles (samples the color of this at the UV position of the mesh section it was emitted from) |
| `WrapMode` | **[WrapMode](https://wiki.resonite.com/Type:WrapMode "Type:WrapMode")** | How to wrap the UV sample coordinates of the mesh. |
| `UVOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to offset the UV sample position of `ColorTexture` |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale the UV sample position of `ColorTexture` |
| `ClipRect` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect") >** | The rectangle to discard UV coordinates if they end up outside this range. Kind of like a UV discard. |
| `Skin` | **[SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer")** | The skinned mesh renderer to emit from. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SkinnedMeshEmitter&oldid=104575](https://wiki.resonite.com/index.php?title=Component:SkinnedMeshEmitter&oldid=104575)"

Contents