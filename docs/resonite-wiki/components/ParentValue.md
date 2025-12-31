# Component:ParentValue

> Source: https://wiki.resonite.com/Component:ParentValue

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/26/ParentValue%601Component.png/510px-ParentValue%601Component.png)](https://wiki.resonite.com/File:ParentValue%601Component.png) **ParentValue<float>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ParentValue<T>** component provides a [value type](https://wiki.resonite.com/Value_type "Value type") for the [parent value](https://wiki.resonite.com/Parent_value "Parent value") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Tag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Tag of the parent value. Compatible [ParentValueLink](https://wiki.resonite.com/Component:ParentValueLink "Component:ParentValueLink") components on the slot's immediate children must have the same tag. |
| `Value` | **T** | The value of the parent value associated with the `Tag` and type. |

Fields
Collapse

## Usage

When this component is on a slot, all immediate children are part of its parent value system. Any immediate children of the slot with a [ParentValueLink](https://wiki.resonite.com/Component:ParentValueLink "Component:ParentValueLink") component that matches the type and `Tag` of this component will be linked to the `Value` provided by this component.

This can be especially useful for [Snapper](https://wiki.resonite.com/Component:Snapper "Component:Snapper")/ [SnapTarget](https://wiki.resonite.com/Component:SnapTarget "Component:SnapTarget") systems.

## Examples

## See Also

- [Component:ParentReference](https://wiki.resonite.com/Component:ParentReference "Component:ParentReference"), for [reference types](https://wiki.resonite.com/Reference_types "Reference types").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ParentValue&oldid=97659](https://wiki.resonite.com/index.php?title=Component:ParentValue&oldid=97659)"

Contents