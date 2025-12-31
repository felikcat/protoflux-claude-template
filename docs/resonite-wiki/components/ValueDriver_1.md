# Component:ValueDriver`1

> Source: https://wiki.resonite.com/Component:ValueDriver`1

(Redirected from [Component:ValueDriver\`1](https://wiki.resonite.com/index.php?title=Component:ValueDriver%601&redirect=no "Component:ValueDriver`1"))

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/50/ValueDriver%601Component.png/510px-ValueDriver%601Component.png)](https://wiki.resonite.com/File:ValueDriver%601Component.png) **ValueDriver<T>** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueDriver<T>** component continuously copies the value of the source [IValue](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") to the target [field](https://wiki.resonite.com/Type:IField "Type:IField") every [update](https://wiki.resonite.com/Update "Update"). The source and target types must be [value types](https://wiki.resonite.com/Value_types "Value types").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ValueSource` | **[IValue\`1](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") <T>** | The value field to get a value from. |
| `DriveTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The value field to set to the value of `ValueSource`. |

Fields
Collapse

## Usage

This component ensures that the value in the `DriveTarget` is equal to the value in the `ValueSource` field. To do this, it [drives](https://wiki.resonite.com/Drives "Drives") the `DriveTarget` field to give it exclusive access to the value, then it starts writing the value from the `ValueSource` field to the target field every update.

This is distinct from [ValueCopy](https://wiki.resonite.com/Component:ValueCopy "Component:ValueCopy"), as it allows sourcing from [IValue](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") elements instead of just [IField](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") elements. It also does not have any `WriteBack` meachanism of any kind. Generally, ValueCopy should be used whenever possible, as it only updates the target field whenever the source field changes instead of every update.

## See also

- [Component:ValueCopy](https://wiki.resonite.com/Component:ValueCopy "Component:ValueCopy")
- [Component:ValueMultiDriver](https://wiki.resonite.com/Component:ValueMultiDriver "Component:ValueMultiDriver") to form this relation to multiple target fields.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueDriver&oldid=113066](https://wiki.resonite.com/index.php?title=Component:ValueDriver&oldid=113066)"

Contents