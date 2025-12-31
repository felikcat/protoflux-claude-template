# Component:ReferenceCast

> Source: https://wiki.resonite.com/Component:ReferenceCast

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ReferenceCast&diff=96504) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/19/ReferenceCast%602Component.png/510px-ReferenceCast%602Component.png)](https://wiki.resonite.com/File:ReferenceCast%602Component.png) **Reference Cast\`2** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ReferenceCast** component can be used to try to take a type and change it to another type. This performs a C# cast which requires the types to be compatible for casting to make a result.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **I** | The source type to convert |
| `Target` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") <O>** | The target field. Casts `Source` to this fields type, and then uses the result to drive this field. |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to allow changes to the `Target` to update `Source` instead of discarding the change. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |

Fields
Collapse

## Usage

This is a way of changing a type without using [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux"). Attaching this component can be difficult, so you should be familiar with [Complex Types in Components](https://wiki.resonite.com/Complex_Types_in_Components "Complex Types in Components"). Keep in mind this does a C# Cast, which does not work with many different conversions.

## Examples

## See Also

- [ProtoFlux:Object Cast](https://wiki.resonite.com/ProtoFlux:Object_Cast "ProtoFlux:Object Cast")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceCast&oldid=96504](https://wiki.resonite.com/index.php?title=Component:ReferenceCast&oldid=96504)"

Contents