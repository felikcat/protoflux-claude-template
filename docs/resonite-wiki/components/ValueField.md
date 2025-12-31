# Component:ValueField

> Source: https://wiki.resonite.com/Component:ValueField

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ValueField&diff=95254) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/dd/ValueField%601Component.png/510px-ValueField%601Component.png)](https://wiki.resonite.com/File:ValueField%601Component.png) **Value Field\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The ValueField component contains a single field of a specific datatype that is selected when the component is attached.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Value` | **T** | The value this component is storing. |

Fields
Collapse

## Usage

The ValueField component can be used to store a single value on a slot that can be edited from the [inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector"), or with other [components](https://wiki.resonite.com/Components "Components") and [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux"). However, in cases where you want to be able to dynamically reference the value instead of directly referencing it, you may be better off using a [dynamic variable](https://wiki.resonite.com/DynamicValueVariable%601_(Component) "DynamicValueVariable`1 (Component)"), and in use cases where you want to easily reference and edit a value within a [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") script while still exposing that value to the data model, you may want to use the [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") node.

## Examples

[![](https://wiki.resonite.com/images/thumb/5/59/Value_Field_Demo.png/300px-Value_Field_Demo.png)](https://wiki.resonite.com/File:Value_Field_Demo.png) A ValueField<floatQ> being used as the input of a ValueCopy<floatQ>

A ValueField could be used when another [component](https://wiki.resonite.com/Components "Components") requires an input of an external value.

## See Also

- [Component:TypeField](https://wiki.resonite.com/Component:TypeField "Component:TypeField")
- [Component:ReferenceField\`1](https://wiki.resonite.com/Component:ReferenceField%601 "Component:ReferenceField`1")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueField&oldid=95254](https://wiki.resonite.com/index.php?title=Component:ValueField&oldid=95254)"

Contents