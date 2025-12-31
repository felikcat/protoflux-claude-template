# Component:ValueCopy

> Source: https://wiki.resonite.com/Component:ValueCopy

Collapse **Component image**

[File:ValueCopy\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ValueCopy%601Component.png "File:ValueCopy`1Component.png") **Value Copy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueCopy** component is used to ensure that a value from one [field](https://wiki.resonite.com/Type:IField "Type:IField") is the same as another field via a one-way relation or a two-way relation with writeback. The source and target types must be [value types](https://wiki.resonite.com/Value_types "Value types").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The source to copy the value from. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The target to copy the value to. |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allow Target to write back to Source. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |

Fields
Collapse

## Usage

This component ensures that the value in the `Target` field is equal to the value in the `Source` field. To do this, it [drives](https://wiki.resonite.com/Drives "Drives") the `Target` field to give it exclusive access to the value, then whenever the value in the `Source` field updates, it will write the new value to the `Target` field.

When `WriteBack` is enabled, the target field will have the ability to be changed. Changes made to the target field will then be written back to the source field.

Using a ValueCopy from a field to itself will essentially make the field read-only. If WriteBack is enabled, it presents an interesting combination of the locality of drives and writing of values: It will make the value of the field local to each individual user. This may be used as a version of [ValueUserOverride](https://wiki.resonite.com/Component:ValueUserOverride "Component:ValueUserOverride") that doesn't do any kind of network writes, but it should be noted that users joining the session will first receive the value from the host user before it gets changed. As such, it should only be used when the value doesn't quite matter specifically or gets updated frequently.

## Examples

- [![A ValueField<int>'s Value is being driven to be 7 from another ValueField<int>'s Value. The one in pink is the one being driven.](https://wiki.resonite.com/images/thumb/d/df/ValueCopyExample2.png/120px-ValueCopyExample2.png)](https://wiki.resonite.com/File:ValueCopyExample2.png "A ValueField<int>'s Value is being driven to be 7 from another ValueField<int>'s Value. The one in pink is the one being driven.")

A ValueField< [int](https://wiki.resonite.com/Type:Int "Type:Int") >'s Value is being driven to be 7 from another ValueField<int>'s Value. The one in pink is the one being driven.

- [![A ValueCopy with WriteBack enabled. The target field is being edited to 4, which changes the source field as well.](https://wiki.resonite.com/images/thumb/a/ae/ValueCopyExample3.png/120px-ValueCopyExample3.png)](https://wiki.resonite.com/File:ValueCopyExample3.png "A ValueCopy with WriteBack enabled. The target field is being edited to 4, which changes the source field as well.")

A ValueCopy with `WriteBack` enabled. The target field is being edited to 4, which changes the source field as well.

- [![A ValueField<int>'s Value is being self driven with a WriteBack. Changes to this value will be local.](https://wiki.resonite.com/images/thumb/4/4e/ValueCopyExample1.png/120px-ValueCopyExample1.png)](https://wiki.resonite.com/File:ValueCopyExample1.png "A ValueField<int>'s Value is being self driven with a WriteBack. Changes to this value will be local.")

A ValueField< [int](https://wiki.resonite.com/Type:Bool "Type:Bool") >'s Value is being self driven with a WriteBack. Changes to this value will be local.


## See also

- [Component:ReferenceCopy](https://wiki.resonite.com/Component:ReferenceCopy "Component:ReferenceCopy") for the same behavior but with [reference types](https://wiki.resonite.com/Reference_types "Reference types").
- [Component:ValueMultiDriver](https://wiki.resonite.com/Component:ValueMultiDriver "Component:ValueMultiDriver") for forming this relation to multiple target fields.
- [Component:ValueDriver](https://wiki.resonite.com/Component:ValueDriver "Component:ValueDriver") for continuously updating a field from an [IValue](https://wiki.resonite.com/Type:IValue "Type:IValue") source rather than a field.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueCopy&oldid=113067](https://wiki.resonite.com/index.php?title=Component:ValueCopy&oldid=113067)"

Contents