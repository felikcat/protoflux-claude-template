# Component:MinMaxValueSpatialVariableDriver

> Source: https://wiki.resonite.com/Component:MinMaxValueSpatialVariableDriver

Collapse **Component image**

[File:MinMaxValueSpatialVariableDriver\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=MinMaxValueSpatialVariableDriver%601Component.png "File:MinMaxValueSpatialVariableDriver`1Component.png") **Min Max Value Spatial Variable Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Min Max Value Spatial Variable Driver\`1** component drives fields with the min and max possible values of the spatial variables it is currently sampling. If there's no spatial variables, Min/Max will be the Max/Min possible values for that datatype

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MinDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The field to drive with the minimum possible value that could be sampled from all the spatial variables that this sampler is sampling from. |
| `MaxDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The field to drive with the maximum possible value that could be sampled from all the spatial variables that this sampler is sampling from. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The variable name to sample for from the point this component's slot is at. |

Fields
Collapse

## Usage

Attach to a slot and provide a field to drive and a variable name. the slot this component is on acts as the position for sampling variable values.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MinMaxValueSpatialVariableDriver&oldid=101132](https://wiki.resonite.com/index.php?title=Component:MinMaxValueSpatialVariableDriver&oldid=101132)"

Contents