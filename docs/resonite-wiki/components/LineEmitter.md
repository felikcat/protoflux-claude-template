# Component:LineEmitter

> Source: https://wiki.resonite.com/Component:LineEmitter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b5/LineEmitterComponent.png/510px-LineEmitterComponent.png)](https://wiki.resonite.com/File:LineEmitterComponent.png) **Line Emitter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LineEmitter** component is used with particle systems (see [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")) to create particles from a straight 3d line made from two points.

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
| `Point0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Point 1 of the line for this Emitter drawn between two points. |
| `Point1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Point 2 of the line for this Emitter drawn between two points. |
| `Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The starting Color multiplier for particles emitted from this Emitter when being emitted nearest to `Point0`. |
| `Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The starting Color multiplier for particles emitted from this Emitter when being emitted nearest to `Point1`. |
| `DirectionMode` | **[LineEmitterDirection](https://wiki.resonite.com/index.php?title=Type:LineEmitterDirection&action=edit&redlink=1 "Type:LineEmitterDirection (page does not exist)")** | How to handle the direction when emitting particles from the line. |
| `Direction0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction particles should go when being emitted nearest to `Point0`. |
| `Direction1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction particles should go when being emitted nearest to `Point1`. |
| `UpDirection` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction that should be considered up for this line. |
| `RandomDirectionWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to randomize the velocity of new particles (this is a magnitude) |
| `DirectionPostTransform` | **[Float3x3](https://wiki.resonite.com/Type:Float3x3 "Type:Float3x3")** | The direction the particles should face as an extra matrix transform after the final particle starting direction has been calculated. |

Fields
Collapse

## Usage

## Examples

## See Also

- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LineEmitter&oldid=104585](https://wiki.resonite.com/index.php?title=Component:LineEmitter&oldid=104585)"

Contents