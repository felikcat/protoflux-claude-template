# Component:LegacyAdapter

> Source: https://wiki.resonite.com/Component:LegacyAdapter

Collapse **Component image**

[File:LegacyAdapterComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LegacyAdapterComponent.png "File:LegacyAdapterComponent.png") **Legacy Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Legacy Adapter** component is used in converted legacy particle systems that were converted to [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust") as part of [The Performance Updates](https://wiki.resonite.com/The_Performance_Updates "The Performance Updates").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ForceDirection` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use force direction. |
| `ForcedDirection` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The forced direction. |
| `DirectionMode` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[LineEmitterDirection](https://wiki.resonite.com/index.php?title=Type:LineEmitterDirection&action=edit&redlink=1 "Type:LineEmitterDirection (page does not exist)")** | `ForceDirection` and `ForcedDirection` converted to PhotonDust direction mode. |
| `Direction0` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | `ForceDirection` and `ForcedDirection` converted to PhotonDust direction vector. |
| `Direction1` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | `ForceDirection` and `ForcedDirection` converted to PhotonDust direction vector. |

Fields
Collapse

## Usage

Not used directly by the user. part of legacy content.

## Examples

Found in legacy content.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyAdapter&oldid=99040](https://wiki.resonite.com/index.php?title=Component:LegacyAdapter&oldid=99040)"

Contents