# Component:LegacyAlignmentSizingAdapter

> Source: https://wiki.resonite.com/Component:LegacyAlignmentSizingAdapter

Collapse **Component image**

[File:LegacyAlignmentSizingAdapterComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LegacyAlignmentSizingAdapterComponent.png "File:LegacyAlignmentSizingAdapterComponent.png") **Legacy Alignment Sizing Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyAlignmentSizingAdapter** component is used in converted legacy particle systems that were converted to [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust") as part of [The Performance Updates](https://wiki.resonite.com/The_Performance_Updates "The Performance Updates").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LengthScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The original length scale from legacy content. |
| `VelocityScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The original velocity scale from legacy content. |
| `Alignment` | **[LegacyParticleAlignment](https://wiki.resonite.com/Type:LegacyParticleAlignment "Type:LegacyParticleAlignment")** | The original alignment from legacy content. |
| `ParticleMesh` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh") >>** | The particle mesh this is using. |
| `UsingStretch` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate this value, and can be used in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `RotationSimulator` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `OrientByVelocity` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `PivotModule` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `UseLocalRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `SizeModifierEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `SizeOffsetByvelocityEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `OrientUp` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `LengthSizeMultiplier` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `VelocitySizeMultiplier` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `PivotMultiplier` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `BillboardAlignment` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[BillboardRenderBufferRenderer.BillboardAlignment](https://wiki.resonite.com/Component:BillboardRenderBufferRenderer#BillboardAlignment "Component:BillboardRenderBufferRenderer")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |
| `MeshAlignment` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[MeshRenderBufferRenderer.MeshAlignment](https://wiki.resonite.com/Component:MeshRenderBufferRenderer#MeshAlignment "Component:MeshRenderBufferRenderer")** | `LengthScale`, `VelocityScale`, and `Alignment` are used to generate the drive value for the target field specified in this, and is used to drive a field of the same name on another component in [PhotonDust](https://wiki.resonite.com/PhotonDust "PhotonDust"). |

Fields
Collapse

## Usage

Not used directly by the user. don't use this to make new content!

## Examples

Used in legacy content for particle systems.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyAlignmentSizingAdapter&oldid=99041](https://wiki.resonite.com/index.php?title=Component:LegacyAlignmentSizingAdapter&oldid=99041)"

Contents