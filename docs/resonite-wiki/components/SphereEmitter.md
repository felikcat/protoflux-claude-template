# Component:SphereEmitter

> Source: https://wiki.resonite.com/Component:SphereEmitter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/61/SphereEmitterComponent.png/510px-SphereEmitterComponent.png)](https://wiki.resonite.com/File:SphereEmitterComponent.png) **Sphere Emitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SphereEmitter** component is used to create particles in a particle system (See [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")). This Emitter emits particles from a sphere shape.

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the sphere shape this is emitting from. |
| `EmitFromShell` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enable emitting particles on the outside of the shape instead of from any point within the volume. |
| `DirectionMode` | **[SphereEmitterDirection](https://wiki.resonite.com/index.php?title=Type:SphereEmitterDirection&action=edit&redlink=1 "Type:SphereEmitterDirection (page does not exist)")** | How particles should be oriented when emitting from the Sphere shape. |
| `RandomDirectionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to randomize the velocity of new particles (this is a magnitude) |
| `ForcedDirection` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Which direction in local space to shoot particles emitted by this emitter. |
| `DirectionTransformMode` | **[DirectionTransformMode](https://wiki.resonite.com/index.php?title=Type:DirectionTransformMode&action=edit&redlink=1 "Type:DirectionTransformMode (page does not exist)")** | How to determine the transform of the particles made by this emitter at start. |
| `DirectionReferencePoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point to use as a reference point when orienting particles upon emission. |
| `DirectionPostTransform` | **[Float3x3](https://wiki.resonite.com/Type:Float3x3 "Type:Float3x3")** | The direction the particles should face as an extra matrix transform after the final particle starting direction has been calculated. |

Fields
Collapse

## Usage

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SphereEmitter&oldid=104589](https://wiki.resonite.com/index.php?title=Component:SphereEmitter&oldid=104589)"

Contents