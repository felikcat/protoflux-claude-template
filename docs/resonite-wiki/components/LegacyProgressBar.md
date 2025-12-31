# Component:LegacyProgressBar

> Source: https://wiki.resonite.com/Component:LegacyProgressBar

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7d/LegacyProgressBarComponent.png/510px-LegacyProgressBarComponent.png)](https://wiki.resonite.com/File:LegacyProgressBarComponent.png) **Legacy Progress Bar** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyProgressBar** component was used in old progress bars for importing items or for cloud storage indicators. This should not be used for new content and should be removed when possible.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Style` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle") >** | The source of the legacy color styles for this component. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `IsEnabledField` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this Legacy UI element is enabled and usable. |
| `Progress` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How close the item is to being imported. |
| `BarColorField` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the loading bar. |
| `ContainerColorField` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the container of the loading bar. |
| `WidthField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of the UI. |
| `HeightField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the UI. |
| `ThicknessField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of the UI. |
| `SlantField` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How beveled the UI edges are. |
| `_barMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh used for the progress bar. |
| `_containerMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh used for the UI container. |
| `_barMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material used for the progress bar. |
| `_containerMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material used for the UI container. |
| `_barPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the bar. |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field of the collider size for the UI. |

Fields
Collapse

## Usage

Just dont.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyProgressBar&oldid=99025](https://wiki.resonite.com/index.php?title=Component:LegacyProgressBar&oldid=99025)"

Contents