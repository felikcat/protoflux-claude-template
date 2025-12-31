# Component:CircleEmitter

> Source: https://wiki.resonite.com/Component:CircleEmitter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0b/CircleEmitterComponent.png/510px-CircleEmitterComponent.png)](https://wiki.resonite.com/File:CircleEmitterComponent.png) **Circle Emitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Circle emitters are used with [Particle Systems](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem") to emit new particles into the system from a circle shaped source.

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the circle is. |
| `Scale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The size of the circle on the x and y separately. used to make elipses. |
| `EmitFromShell` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enable emitting particles on the outside of the shape instead of from any point within the volume. |
| `CircleAlignment` | **[CircleEmitterAlignment](https://wiki.resonite.com/index.php?title=Type:CircleEmitterAlignment&action=edit&redlink=1 "Type:CircleEmitterAlignment (page does not exist)")** | How to align the particles via the circle on start. |
| `DirectionMode` | **[CircleEmitterDirection](https://wiki.resonite.com/index.php?title=Type:CircleEmitterDirection&action=edit&redlink=1 "Type:CircleEmitterDirection (page does not exist)")** | How to emit particles from the circle. |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Which direction in local space to shoot particles emitted by this emitter. |
| `DirectionTransformMode` | **[DirectionTransformMode](https://wiki.resonite.com/index.php?title=Type:DirectionTransformMode&action=edit&redlink=1 "Type:DirectionTransformMode (page does not exist)")** | How to determine the transform of the particles made by this emitter at start. |
| `RandomDirectionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to randomize the velocity of new particles (this is a magnitude) |
| `DirectionPostTransform` | **[Float3x3](https://wiki.resonite.com/Type:Float3x3 "Type:Float3x3")** | The direction the particles should face as an extra matrix transform after the final particle starting direction has been calculated. |

Fields
Collapse

## Usage

Used in particle systems to create new particles

## Examples

## See Also

- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CircleEmitter&oldid=104588](https://wiki.resonite.com/index.php?title=Component:CircleEmitter&oldid=104588)"

Contents