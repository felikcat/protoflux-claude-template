# Component:ProtoFluxWireManager

> Source: https://wiki.resonite.com/Component:ProtoFluxWireManager

Collapse **Component image**

[File:ProtoFluxWireManagerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFluxWireManagerComponent.png "File:ProtoFluxWireManagerComponent.png") **Proto Flux Wire Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtoFluxWireManager** component is used to drive the visual elements of protoflux wires which connect protoflux nodes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ConnectPoint` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The point this is supposed to be pointing to. |
| `Type` | **[WireType](https://wiki.resonite.com/Type:WireType "Type:WireType")** | The type of wire this is supposed to be showing. |
| `Width` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width this wire should be. |
| `StartColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color this wire should start at. usually used for async impulse wires. |
| `EndColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The end color this wire should end at. usually used for async impulse wires. |
| `DeleteHighlight` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to delete the highlight visual. |
| `_wireMesh` | **[StripeWireMesh](https://wiki.resonite.com/Component:StripeWireMesh "Component:StripeWireMesh")** | The stripe mesh this is modifying. |
| `_renderer` | **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | The renderer of the stripe mesh this is modifying. |
| `_collider` | **[MeshCollider](https://wiki.resonite.com/Component:MeshCollider "Component:MeshCollider")** | The collider of this stripe mesh visual. |
| `_targetPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the target position for the stripe mesh. |
| `_targetTangent` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the target tangent for the stripe mesh. |
| `_targetOrientation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive with the target orientation for the stripe mesh. |
| `_targetWidth` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the target width for the stripe mesh. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxWireManager&oldid=106528](https://wiki.resonite.com/index.php?title=Component:ProtoFluxWireManager&oldid=106528)"

Contents