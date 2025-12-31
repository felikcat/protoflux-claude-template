# Component:BoxEmitter

> Source: https://wiki.resonite.com/Component:BoxEmitter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d4/BoxEmitterComponent.png/510px-BoxEmitterComponent.png)](https://wiki.resonite.com/File:BoxEmitterComponent.png) **Box Emitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Box emitter is a component that is used in conjunction with [Particle System](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem") and [Particle Style](https://wiki.resonite.com/Component:ParticleStyle "Component:ParticleStyle"). It allows for adding particles into a Particle system with a rate, and does them inside or along the outside of the box area specified. The particle starting colors are lerped based on what corner of the cube the particle generated is closest to.

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
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size of this box emitter. |
| `EmitFromShell` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enable emitting particles on the outside of the shape instead of from any point within the volume. |
| `DirectionMode` | **[BoxEmitterDirection](https://wiki.resonite.com/index.php?title=Type:BoxEmitterDirection&action=edit&redlink=1 "Type:BoxEmitterDirection (page does not exist)")** | What direction to shoot the particles in from the box. |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Which direction in local space to shoot particles emitted by this emitter. |
| `DirectionTransformMode` | **[DirectionTransformMode](https://wiki.resonite.com/index.php?title=Type:DirectionTransformMode&action=edit&redlink=1 "Type:DirectionTransformMode (page does not exist)")** | How to determine the transform of the particles made by this emitter at start. |
| `RandomDirectionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to randomize the velocity of new particles (this is a magnitude) |
| `DirectionPostTransform` | **[Float3x3](https://wiki.resonite.com/Type:Float3x3 "Type:Float3x3")** | The direction the particles should face as an extra matrix transform after the final particle starting direction has been calculated. |
| `Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the cube on corner (-x,-z,-y) |
| `Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the cube on corner (+x,-z,-y) |
| `Color2` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the cube on corner (+x,+z,-y) |
| `Color3` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the cube on corner (-x,+z,-y) |
| `Color4` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the cube on corner (-x,-z,+y) |
| `Color5` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the cube on corner (+x,-z,+y) |
| `Color6` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the cube on corner (+x,+z,+y) |
| `Color7` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the cube on corner (-x,+z,+y) |

Fields
Collapse

## Usage

Used in creations using particle systems as a source of particles.

## Examples

Useful to make fireflies in an area, for a calming nighttime aura. It can also be used to make leaves fall from trees by making a box around the tree leaves, or as wind particles in a breezy field.

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxEmitter&oldid=104583](https://wiki.resonite.com/index.php?title=Component:BoxEmitter&oldid=104583)"

Contents