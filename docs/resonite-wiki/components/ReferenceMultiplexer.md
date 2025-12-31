# Component:ReferenceMultiplexer

> Source: https://wiki.resonite.com/Component:ReferenceMultiplexer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ad/ReferenceMultiplexer%601Component.png/510px-ReferenceMultiplexer%601Component.png)](https://wiki.resonite.com/File:ReferenceMultiplexer%601Component.png) **Reference Multiplexer\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

ReferenceMultiplexers allow to curate a list of references and [drive](https://wiki.resonite.com/Drive "Drive") a target with one of them.

Unlike [ValueMultiplexers](https://wiki.resonite.com/Component:ValueMultiplexer "Component:ValueMultiplexer") they don't implement [IValue](https://wiki.resonite.com/Type:IValue%601 "Type:IValue`1") and therefore can't be accessed directly within ProtoFlux.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") <T>** | A [SyncRef](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") which is driven with the currently selected reference |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | 0-based index that determines which reference of `References` has been selected; values outside the range `[0;length-1]` are wrapped around internally. |
| `References` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **T** | A list of references which can also individually be driven or written to |
| `AllowWriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Setting this to `true` redirects writes from `Target` to the currently indexed list entry. |

Fields
Collapse

## Usage

The component behaves similar to a [ReferenceCopy](https://wiki.resonite.com/Component:ReferenceCopy "Component:ReferenceCopy") with the list entry indicated by `Index` as its `Source`.
Changes to `Index` or the list entries will affect `Target` whenever the drive is evaluated.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceMultiplexer&oldid=106256](https://wiki.resonite.com/index.php?title=Component:ReferenceMultiplexer&oldid=106256)"

Contents