# Component:BooleanSpatialVariableDriver

> Source: https://wiki.resonite.com/Component:BooleanSpatialVariableDriver

Collapse **Component image**

[File:BooleanSpatialVariableDriverComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=BooleanSpatialVariableDriverComponent.png "File:BooleanSpatialVariableDriverComponent.png") **Boolean Spatial Variable Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Boolean Spatial Variable Driver** component is specifically for boolean values, which combines all the found bool spatial values at given point

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Drive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with the combined values of all the bools at the sampled slot point. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The variable name to sample. |
| `Mode` | **[BooleanSpatialVariableMode](https://wiki.resonite.com/Type:BooleanSpatialVariableMode "Type:BooleanSpatialVariableMode")** | How to aggrigate values to determine the final result. |
| `DefaultValue` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The value to default to when no value can be sampled. |

Fields
Collapse

## Usage

attach to a slot for it to use as the sample point. then it will sample spatial areas around it to get it's value.

## Examples

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BooleanSpatialVariableDriver&oldid=101079](https://wiki.resonite.com/index.php?title=Component:BooleanSpatialVariableDriver&oldid=101079)"

Contents