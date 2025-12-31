# Component:CylinderEmitter

> Source: https://wiki.resonite.com/Component:CylinderEmitter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9e/CylinderEmitterComponent.png/510px-CylinderEmitterComponent.png)](https://wiki.resonite.com/File:CylinderEmitterComponent.png) **Cylinder Emitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CylinderEmitter** component is used to emit particles in PhotonDust.

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the emitting cylinder shape |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the emitting cylinder shape. |
| `EmitFromShell` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Enable emitting particles on the outside of the shape instead of from any point within the volume. |
| `ExcludeCaps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to exclude the ends of the cylinder when emitting particles. |
| `DirectionMode` | **[CylinderEmitterDirection](https://wiki.resonite.com/index.php?title=Type:CylinderEmitterDirection&action=edit&redlink=1 "Type:CylinderEmitterDirection (page does not exist)")** | How to emit particles from the cylinder. |
| `CapsDirectionMode` | **[CylinderEmitterCapsDirection](https://wiki.resonite.com/index.php?title=Type:CylinderEmitterCapsDirection&action=edit&redlink=1 "Type:CylinderEmitterCapsDirection (page does not exist)")** | how to emit particles from the cylinder caps. |
| `RandomDirectionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to randomize the velocity of new particles (this is a magnitude) |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Which direction in local space to shoot particles emitted by this emitter. |
| `DirectionTransformMode` | **[DirectionTransformMode](https://wiki.resonite.com/index.php?title=Type:DirectionTransformMode&action=edit&redlink=1 "Type:DirectionTransformMode (page does not exist)")** | How to handle the direction when emitting particles. |
| `DirectionPostTransform` | **[Float3x3](https://wiki.resonite.com/Type:Float3x3 "Type:Float3x3")** | The direction particles should be when spawned post transform using a matrix. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CylinderEmitter&oldid=104584](https://wiki.resonite.com/index.php?title=Component:CylinderEmitter&oldid=104584)"

Contents