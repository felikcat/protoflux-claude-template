# Component:LegacyRotationAdapter

> Source: https://wiki.resonite.com/Component:LegacyRotationAdapter

Collapse **Component image**

[File:LegacyRotationAdapterComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LegacyRotationAdapterComponent.png "File:LegacyRotationAdapterComponent.png") **Legacy Rotation Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyRotationAdapter** component can be used to convert legacy rotation values to the new particle system values.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the converted value. |
| `Value` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The original rotation value. |
| `ParticleMesh` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh") >>** | The mesh particle that was used with the original if any. |
| `UsingStretch` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | Whether or not stretch was used with the particle. |

Fields
Collapse

## Usage

Not used directly by the user. Used in legacy content.

## Examples

Used in legacy content.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyRotationAdapter&oldid=99180](https://wiki.resonite.com/index.php?title=Component:LegacyRotationAdapter&oldid=99180)"

Contents