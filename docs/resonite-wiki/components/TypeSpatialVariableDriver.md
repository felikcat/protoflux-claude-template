# Component:TypeSpatialVariableDriver

> Source: https://wiki.resonite.com/Component:TypeSpatialVariableDriver

Collapse **Component image**

[File:TypeSpatialVariableDriverComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=TypeSpatialVariableDriverComponent.png "File:TypeSpatialVariableDriverComponent.png") **Type Spatial Variable Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Type Spatial Variable Driver** component is part of the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. It will drive a field with value sampled at the current global position of the slot it's on. The value used is one with highest priority

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Drive` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The field to drive with the sampled value. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The variable name to sample for. |
| `DefaultType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The value to default to if no variable is found from sampling at the point of the slot this component is on. |

Fields
Collapse

## Usage

Attach to a slot and provide a field to drive and a variable name. the slot this component is on acts as the position for sampling variable values.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TypeSpatialVariableDriver&oldid=101130](https://wiki.resonite.com/index.php?title=Component:TypeSpatialVariableDriver&oldid=101130)"

Contents