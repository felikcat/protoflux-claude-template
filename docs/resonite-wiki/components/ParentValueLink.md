# Component:ParentValueLink

> Source: https://wiki.resonite.com/Component:ParentValueLink

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/64/ParentValueLink%601Component.png/510px-ParentValueLink%601Component.png)](https://wiki.resonite.com/File:ParentValueLink%601Component.png) **ParentValueLink<float>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ParentValueLink<T>** component [drives](https://wiki.resonite.com/Drives "Drives") a [field](https://wiki.resonite.com/Field "Field") depending on the value of a compatible [ParentValue](https://wiki.resonite.com/Component:ParentValue "Component:ParentValue") as part of a [parent value](https://wiki.resonite.com/Parent_value "Parent value") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MatchTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The tag to search for on the slot's immediate parent. Compatible [ParentValue](https://wiki.resonite.com/Component:ParentValue "Component:ParentValue") components must have the same `Tag`. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The field to drive using the value of the linked parent. |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If `True`, any writes to the driven field will be propagated back to the `Value` provided by the ParentValue. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |
| `DefaultValue` | **T** | Default value to use if the component can not find a compatible ParentValue. |

Fields
Collapse

## Usage

Upon a change of parent, this component will search for ParentValue components on the slot's immediate parent that have a matching type and tag. If it can find such a component and link to it, it will drive the `Target` field based on the `Value` of the ParentValue. If it can not find such a component, it will use the `DefaultValue` value.

## Examples

## See Also

- [Component:ParentReferenceLink](https://wiki.resonite.com/Component:ParentReferenceLink "Component:ParentReferenceLink"), for [reference types](https://wiki.resonite.com/Reference_types "Reference types")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ParentValueLink&oldid=97658](https://wiki.resonite.com/index.php?title=Component:ParentValueLink&oldid=97658)"

Contents