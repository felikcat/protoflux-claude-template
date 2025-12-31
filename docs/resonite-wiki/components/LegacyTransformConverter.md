# Component:LegacyTransformConverter

> Source: https://wiki.resonite.com/Component:LegacyTransformConverter

Collapse **Component image**

[File:LegacyTransformConverterComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LegacyTransformConverterComponent.png "File:LegacyTransformConverterComponent.png") **Legacy Transform Converter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Legacy Transform Converter** component converts transforms for legacy content to the new [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Transform` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3x3](https://wiki.resonite.com/Type:Float3x3 "Type:Float3x3")** | The transform field to drive with a converted value. |
| `Emitter` | **[SphereEmitter](https://wiki.resonite.com/Component:SphereEmitter "Component:SphereEmitter")** | The emitter to make conversions with. |

Fields
Collapse

## Usage

Not to be used in new content. Acts as a Legacy content converter.

## Examples

Used in old content.

## See Also

- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyTransformConverter&oldid=100980](https://wiki.resonite.com/index.php?title=Component:LegacyTransformConverter&oldid=100980)"

Contents