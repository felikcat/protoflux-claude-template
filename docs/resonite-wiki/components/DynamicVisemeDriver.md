# Component:DynamicVisemeDriver

> Source: https://wiki.resonite.com/Component:DynamicVisemeDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c0/DynamicVisemeDriverComponent.png/510px-DynamicVisemeDriverComponent.png)](https://wiki.resonite.com/File:DynamicVisemeDriverComponent.png) **Dynamic Viseme Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DynamicVisemeDriver** component allows using a viseme analyser to drive Float values. It allows for combinations of visemes with weights to drive a Float, and said Float may be a shapekey.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[VisemeAnalyzer](https://wiki.resonite.com/Component:VisemeAnalyzer "Component:VisemeAnalyzer")** | The analyzer making viseme data. |
| `MouthTrackingSource` | **[IMouthTrackingSourceComponent](https://wiki.resonite.com/Type:IMouthTrackingSourceComponent "Type:IMouthTrackingSourceComponent")** | The source of mouth tracking to influence viseme data. |
| `VoiceMouthSupressWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much audio supresses the effect of the `MouthTrackingSource` data. |
| `Drivers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[DynamicVisemeDriver.TargetDriver](https://wiki.resonite.com/Component:DynamicVisemeDriver#TargetDriver)** | A list of drivers that use the `Source` and `MouthTrackingSource` data to drive their targets. |

Fields
Collapse

## Target Driver

| Name | Type | Description |
| --- | --- | --- |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The float value to drive. May be a shapekey. |
| `Sources` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[VisemeSource](https://wiki.resonite.com/Component:DynamicVisemeDriver#VisemeSource)** | A list of sources to use to drive `Target` |

Fields

## VisemeSource

| Name | Type | Description |
| --- | --- | --- |
| `Viseme` | **[Viseme](https://wiki.resonite.com/Type:Viseme "Type:Viseme")** | The viseme to get Float data from. |
| `Influence` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much `Viseme` should affect `Target`. All instances of this value do not have to add up to 1. The final set of values are normalized with the rest. |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicVisemeDriver&oldid=97479](https://wiki.resonite.com/index.php?title=Component:DynamicVisemeDriver&oldid=97479)"

Contents