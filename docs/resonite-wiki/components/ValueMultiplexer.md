# Component:ValueMultiplexer

> Source: https://wiki.resonite.com/Component:ValueMultiplexer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fa/ValueMultiplexer%601Component.png/510px-ValueMultiplexer%601Component.png)](https://wiki.resonite.com/File:ValueMultiplexer%601Component.png) **Value Multiplexer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueMultiplexer** component allows one to curate a list of values and [drive](https://wiki.resonite.com/Drive "Drive") a target with one of them, much like a multiplexer.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | A field which is driven with the currently selected list value |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | 0-based index that determines which value of `Values` has been selected; values outside the range `[0;length-1]` are wrapped around internally. |
| `Values` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") <T>** | A list of values which can also individually be driven or written to |
| `AllowWriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Setting this to `true` redirects writes from `Target` or from a `Source` representing the selected value to the currently indexed list entry. |

Fields
Collapse

## Usage

The component behaves similar to a [ValueCopy](https://wiki.resonite.com/Component:ValueCopy "Component:ValueCopy") with the list entry indicated by `Index` as the value to output. Changes to `Index` or the list entries will affect `Target` whenever the drive is evaluated.

In addition, the component implements the [IValue](https://wiki.resonite.com/Type:IValue "Type:IValue") interface. This allows the component to be [sourced](https://wiki.resonite.com/ProtoFlux:Source "ProtoFlux:Source") by dragging out the component header with the ProtoFlux tip. This allows one to use the component like an array when sourcing the `Index` field as well. The source of this component will update instantly, as opposed to the drive being limited to once per frame.

## Examples

- [![Array-like access from within ProtoFlux. Note the setting of AllowWriteBack and that you can only access a single value at a time!](https://wiki.resonite.com/images/thumb/d/d2/ValueMultiplexer_ProtoFlux_1.png/540px-ValueMultiplexer_ProtoFlux_1.png)](https://wiki.resonite.com/File:ValueMultiplexer_ProtoFlux_1.png "Array-like access from within ProtoFlux. Note the setting of AllowWriteBack and that you can only access a single value at a time!")

Array-like access from within ProtoFlux. Note the setting of `AllowWriteBack` and that you can only access a single value at a time!

- [![A demonstration of what happens when Index is outside the usual range. (wraps around)](https://wiki.resonite.com/images/thumb/9/9f/ValueMultiplexer_ProtoFlux_Wrapping_Index.png/540px-ValueMultiplexer_ProtoFlux_Wrapping_Index.png)](https://wiki.resonite.com/File:ValueMultiplexer_ProtoFlux_Wrapping_Index.png "A demonstration of what happens when Index is outside the usual range. (wraps around)")

A demonstration of what happens when `Index` is outside the usual range. (wraps around)


## See Also

- [Component:ReferenceMultiplexer](https://wiki.resonite.com/Component:ReferenceMultiplexer "Component:ReferenceMultiplexer")
- [ProtoFlux:Multiplex](https://wiki.resonite.com/ProtoFlux:Multiplex "ProtoFlux:Multiplex")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueMultiplexer&oldid=97817](https://wiki.resonite.com/index.php?title=Component:ValueMultiplexer&oldid=97817)"

Contents