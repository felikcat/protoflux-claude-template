# Component:MeshEmitter

> Source: https://wiki.resonite.com/Component:MeshEmitter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2f/MeshEmitter.png/510px-MeshEmitter.png)](https://wiki.resonite.com/File:MeshEmitter.png) **Mesh Emitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MeshEmitter** component allows for emitting particles from a mesh.

This is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius")

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
| `EmitFrom` | **[MeshEmissionSource](https://wiki.resonite.com/Type:MeshEmissionSource "Type:MeshEmissionSource")** | What parts of the mesh to emit from for the specified mesh. |
| `UseVertexColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to use interpolated vertex colors of the mesh this is emitting from. |
| `DirectionMode` | **[MeshEmitterDirection](https://wiki.resonite.com/index.php?title=Type:MeshEmitterDirection&action=edit&redlink=1 "Type:MeshEmitterDirection (page does not exist)")** | How to determine the emission direction of particles emitted from this mesh. |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Which direction in local space to shoot particles emitted by this emitter. |
| `RandomDirectionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to randomize the velocity of new particles (this is a magnitude) |
| `ColorTexture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to sample from for the particle starting color, which is sampled from the texture via the uv coordinate of the mesh surface the particle was emitted from. |
| `WrapMode` | **[WrapMode](https://wiki.resonite.com/Type:WrapMode "Type:WrapMode")** | How to wrap the texture sampling for the particle color when the uvs are beyond a 0 to 1 range. |
| `UVOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to offset the UVs before sampling for particle color. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How much to scale up/down the UVs before sampling for particle color. |
| `ClipRect` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect") >** | Particles will only emit if the mesh surface uv is within this clip rectangle. |
| `Mesh` | **[Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh")** | The mesh to use for particle emission. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Related Components

- [Component:SkinnedMeshEmitter](https://wiki.resonite.com/Component:SkinnedMeshEmitter "Component:SkinnedMeshEmitter")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshEmitter&oldid=103864](https://wiki.resonite.com/index.php?title=Component:MeshEmitter&oldid=103864)"

Contents