# Component:ConeEmitter

> Source: https://wiki.resonite.com/Component:ConeEmitter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/06/ConeEmitterComponent.png/510px-ConeEmitterComponent.png)](https://wiki.resonite.com/File:ConeEmitterComponent.png) **Cone Emitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ConeEmitter** component is used to create particles via a particle system (see [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")). This Emitter does this in a cone shape.

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
| `BaseRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the cone to emit from. |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the cone to emit from. |
| `EmitFromShell` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enable emitting particles on the outside of the shape instead of from any point within the volume. |
| `DirectionMode` | **[ConeEmitterDirection](https://wiki.resonite.com/index.php?title=Type:ConeEmitterDirection&action=edit&redlink=1 "Type:ConeEmitterDirection (page does not exist)")** | How particles are emitted from the cone. |
| `RandomDirectionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to randomize the velocity of new particles (this is a magnitude) |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Which direction in local space to shoot particles emitted by this emitter. |
| `DirectionTransformMode` | **[DirectionTransformMode](https://wiki.resonite.com/index.php?title=Type:DirectionTransformMode&action=edit&redlink=1 "Type:DirectionTransformMode (page does not exist)")** | How to determine the transform of the particles made by this emitter at start. |
| `RandomDirectionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to randomize the velocity of new particles (this is a magnitude) |
| `DirectionPostTransform` | **[Float3x3](https://wiki.resonite.com/Type:Float3x3 "Type:Float3x3")** | The direction the particles should face as an extra matrix transform after the final particle starting direction has been calculated. |

Fields
Collapse

## Usage

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ConeEmitter&oldid=104587](https://wiki.resonite.com/index.php?title=Component:ConeEmitter&oldid=104587)"

Contents