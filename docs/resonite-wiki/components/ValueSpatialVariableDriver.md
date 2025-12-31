# Component:ValueSpatialVariableDriver

> Source: https://wiki.resonite.com/Component:ValueSpatialVariableDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/44/ValueSpatialVariableDriver%601Component.png/510px-ValueSpatialVariableDriver%601Component.png)](https://wiki.resonite.com/File:ValueSpatialVariableDriver%601Component.png) **Value Spatial Variable Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Value Spatial Variable Driver\`1** component samples from [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") intersecting the slot it is on and gets a value.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Drive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The field to drive with the sampled variable. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | the name of the variable to be sampling for. |
| `DefaultValue` | **T** | The value to default to when no value can be sampled. |

Fields
Collapse

## Usage

Attach to a slot and provide a field to drive and a variable name. the slot this component is on acts as the position for sampling variable values.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueSpatialVariableDriver&oldid=101133](https://wiki.resonite.com/index.php?title=Component:ValueSpatialVariableDriver&oldid=101133)"

Contents