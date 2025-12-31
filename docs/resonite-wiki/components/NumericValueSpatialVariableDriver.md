# Component:NumericValueSpatialVariableDriver

> Source: https://wiki.resonite.com/Component:NumericValueSpatialVariableDriver

Collapse **Component image**

[File:NumericValueSpatialVariableDriver\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=NumericValueSpatialVariableDriver%601Component.png "File:NumericValueSpatialVariableDriver`1Component.png") **Numeric Value Spatial Variable Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Numeric Value Spatial Variable Driver\`1** component works specifically for numeric values and allows for multiple sampling modes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Drive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The field to drive with the resulting value. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The variable name to sample for. |
| `Mode` | **[ValueSpatialVariableMode](https://wiki.resonite.com/Type:ValueSpatialVariableMode "Type:ValueSpatialVariableMode")** | How to interpret the sampled values. |
| `DefaultValue` | **T** | The value to default to if no value can be sampled. |

Fields
Collapse

## Usage

Attach to a slot and provide a field to drive and a variable name. the slot this component is on acts as the position for sampling variable values.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NumericValueSpatialVariableDriver&oldid=101138](https://wiki.resonite.com/index.php?title=Component:NumericValueSpatialVariableDriver&oldid=101138)"

Contents