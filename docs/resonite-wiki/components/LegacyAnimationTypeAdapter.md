# Component:LegacyAnimationTypeAdapter

> Source: https://wiki.resonite.com/Component:LegacyAnimationTypeAdapter

Collapse **Component image**

[File:LegacyAnimationTypeAdapterComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LegacyAnimationTypeAdapterComponent.png "File:LegacyAnimationTypeAdapterComponent.png") **Legacy Animation Type Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyAnimationTypeAdapter** component is used in converted legacy particle systems that were converted to [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust") as part of [The Performance Updates](https://wiki.resonite.com/The_Performance_Updates "The Performance Updates").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[LegacyParticleAnimationType](https://wiki.resonite.com/index.php?title=Type:LegacyParticleAnimationType&action=edit&redlink=1 "Type:LegacyParticleAnimationType (page does not exist)")** | The original animation type from legacy content. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[TextureSheetAnimationType](https://wiki.resonite.com/index.php?title=Type:TextureSheetAnimationType&action=edit&redlink=1 "Type:TextureSheetAnimationType (page does not exist)")** | The target field to drive with the legacy animation values. |
| `AnimationTiles` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") < [Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2") >>** | The field to set to the amount of animation tiles. |
| `AnimationEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether animation should be enabled. |

Fields
Collapse

## Usage

Not used directly by the user. Don't use this in new content!

## Examples

Found in legacy particle content.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyAnimationTypeAdapter&oldid=99042](https://wiki.resonite.com/index.php?title=Component:LegacyAnimationTypeAdapter&oldid=99042)"

Contents