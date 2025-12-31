# Component:ParentReferenceLink

> Source: https://wiki.resonite.com/Component:ParentReferenceLink

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/28/ParentReferenceLink%601Component.png/510px-ParentReferenceLink%601Component.png)](https://wiki.resonite.com/File:ParentReferenceLink%601Component.png) **ParentReferenceLink<Slot>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ParentReferenceLink<T>** component [drives](https://wiki.resonite.com/Drives "Drives") a [field](https://wiki.resonite.com/Field "Field") depending on the value of a compatible [ParentReference](https://wiki.resonite.com/Component:ParentReference "Component:ParentReference") as part of a [parent value](https://wiki.resonite.com/Parent_value "Parent value") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MatchTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The tag to search for on the slot's immediate parent. Compatible [ParentReference](https://wiki.resonite.com/Component:ParentReference "Component:ParentReference") components must have the same `Tag`. |
| `Target` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") <T>** | The field to drive using the value of the linked parent. |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If `True`, any writes to the driven field will be propagated back to the `Reference` provided by the ParentReference. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |
| `DefaultReference` | **T** | Default value to use if the component can not find a compatible ParentReference. |

Fields
Collapse

## Usage

Upon a change of parent, this component will search for ParentReference components on the slot's immediate parent that have a matching type and tag. If it can find such a component and link to it, it will drive the `Target` field based on the `Reference` of the ParentReference. If it can not find such a component, it will use the `DefaultReference` value.

## Examples

## See Also

- [Component:ParentValueLink](https://wiki.resonite.com/Component:ParentValueLink "Component:ParentValueLink"), for [value types](https://wiki.resonite.com/Value_types "Value types")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ParentReferenceLink&oldid=97656](https://wiki.resonite.com/index.php?title=Component:ParentReferenceLink&oldid=97656)"

Contents