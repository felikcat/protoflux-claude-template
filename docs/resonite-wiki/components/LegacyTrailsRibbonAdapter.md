# Component:LegacyTrailsRibbonAdapter

> Source: https://wiki.resonite.com/Component:LegacyTrailsRibbonAdapter

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[File:LegacyTrailsRibbonAdapterComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LegacyTrailsRibbonAdapterComponent.png "File:LegacyTrailsRibbonAdapterComponent.png") **Legacy Trails Ribbon Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Legacy Trails Ribbon Adapter** component is used to convert legacy content from the old particle system driven by Unity to [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TrailsMode` | **[LegacyParticleTrailMode](https://wiki.resonite.com/index.php?title=Type:LegacyParticleTrailMode&action=edit&redlink=1 "Type:LegacyParticleTrailMode (page does not exist)")** | The enum used to control the conversion from legacy trails to [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust"). |
| `ParticleSizeAffectsTrailWidth` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the particle size should affect the trail width. |
| `InheritTrailColorFromParticle` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the trail should inherit color from the particle it is following. |
| `TrailWorldSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the trail is in world or local space. |
| `TrailsModule` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field on a trails module to drive. |
| `RibbonModule` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field on a ribbons module to drive. |
| `RibbonUseParticleSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The use particle size field to drive on a ribbons module. |
| `RibbonUseParticleColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The use particle color field to drive on a ribbons module. |
| `TrailSizeInheritance` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[TrailParticleInheritance](https://wiki.resonite.com/index.php?title=Type:TrailParticleInheritance&action=edit&redlink=1 "Type:TrailParticleInheritance (page does not exist)")** | The use particle size field to drive on a trails module. |
| `TrailColorInheritance` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[TrailParticleInheritance](https://wiki.resonite.com/index.php?title=Type:TrailParticleInheritance&action=edit&redlink=1 "Type:TrailParticleInheritance (page does not exist)")** | The use particle color field to drive on a trails module. |
| `TrailsSpace` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The trails space field to drive on a trails module. |

Fields
Collapse

## Usage

Used in legacy content. do not use in new content.

## Examples

Used in legacy content.

## See Also

- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyTrailsRibbonAdapter&oldid=103800](https://wiki.resonite.com/index.php?title=Component:LegacyTrailsRibbonAdapter&oldid=103800)"

Contents