# Component:OriginRadialForce

> Source: https://wiki.resonite.com/Component:OriginRadialForce

Collapse **Component image**

[File:OriginRadialForceComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=OriginRadialForceComponent.png "File:OriginRadialForceComponent.png") **Origin Radial Force** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Origin Radial Force** component is used with [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") to make particles have force applied on them to make them return to their original starting point over time. This was a personal addition by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Force` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The constant force applied to particles to make them return to where they started. |
| `Mode` | **[RadialForceMode](https://wiki.resonite.com/index.php?title=Type:RadialForceMode&action=edit&redlink=1 "Type:RadialForceMode (page does not exist)")** | how the Radial area and effect for this component is defined. |
| `MinDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from 0 where the minimum force is defined in the force gradient. |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from 0 where the maximum force is defined in the force gradient. |
| `MinForce` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum force value for the gradient. |
| `MaxForce` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum force value for the gradient. |
| `OverrideForceSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space to apply forces for this component in. |

Fields
Collapse

## Usage

Used in [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") systems.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OriginRadialForce&oldid=105350](https://wiki.resonite.com/index.php?title=Component:OriginRadialForce&oldid=105350)"

Contents