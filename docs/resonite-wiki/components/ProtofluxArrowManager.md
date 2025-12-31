# Component:ProtofluxArrowManager

> Source: https://wiki.resonite.com/Component:ProtofluxArrowManager

Collapse **Component image**

[File:ProtofluxArrowManagerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtofluxArrowManagerComponent.png "File:ProtofluxArrowManagerComponent.png") **Protoflux Arrow Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtofluxArrowManager** component is used to drive and create the visuals for arrows pointing from/to variables and where they are being used.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ConnectNode` | _direct_ **[TransformRelayRef](https://wiki.resonite.com/index.php?title=Type:TransformRelayRef&action=edit&redlink=1 "Type:TransformRelayRef (page does not exist)")** | The node the arrow should point to. |
| `TargetSize` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >>** | The size field of the target. |
| `TargetOffset` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >>** | The offset field of the target. |
| `_arrowMesh` | **[ArrowMesh](https://wiki.resonite.com/Component:ArrowMesh "Component:ArrowMesh")** | The arrow mesh this is modifying. |
| `_renderer` | **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | The renderer rendering `_arrowMesh` |
| `_targetVector` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field for the target vector on the arrow mesh. |

Fields
Collapse

## Usage

Not usually used by the user.

## Examples

## See Also

- [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtofluxArrowManager&oldid=106428](https://wiki.resonite.com/index.php?title=Component:ProtofluxArrowManager&oldid=106428)"

Contents