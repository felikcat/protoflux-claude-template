# Component:SizeMultiplierByVelocity

> Source: https://wiki.resonite.com/Component:SizeMultiplierByVelocity

Collapse **Component image**

[File:SizeMultiplierByVelocityComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SizeMultiplierByVelocityComponent.png "File:SizeMultiplierByVelocityComponent.png") **Size Multiplier By Velocity** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Size Multiplier By Velocity** component is used in [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") systems to make particles change size on any given axies based on velocity.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VelocityMultiplier` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The amount to multiply velocity of a particle by before using it as a multiplier. |
| `VelocityMask` | **[Bool3](https://wiki.resonite.com/Type:Bool3 "Type:Bool3")** | Which axies should be included in or excluded from this scaling effect. |
| `MultiplierClampMin` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the minimum value to clamp the current velocity of a particle to before it is used as a scale multiplier. |
| `MultiplierClampMax` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the maximum value to clamp the current velocity of a particle to before it is used as a scale multiplier. |
| `ResultClampMin` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the minimum scale the particle is allowed to be as a final scale. |
| `ResultClampMax` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the maximum scale the particle is allowed to be as a final scale. |

Fields
Collapse

## Usage

Used in particle systems to change particle size by velocity.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SizeMultiplierByVelocity&oldid=106403](https://wiki.resonite.com/index.php?title=Component:SizeMultiplierByVelocity&oldid=106403)"

Contents