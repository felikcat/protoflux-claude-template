# Component:BooleanValueDriver

> Source: https://wiki.resonite.com/Component:BooleanValueDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BooleanValueDriver&diff=113547) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/90/BooleanValueDriver%601Component.png/510px-BooleanValueDriver%601Component.png)](https://wiki.resonite.com/File:BooleanValueDriver%601Component.png) **BooleanValueDriver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BooleanValueDriver** component drives the [Field](https://wiki.resonite.com/Field "Field") in `TargetField` to the value specified in `TrueValue` or `FalseValue` based on `State`.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `State` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The state of this component. Chooses which value to use when driving `TargetField` |
| `TargetField` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **T** | The [Field](https://wiki.resonite.com/Field "Field") to drive |
| `FalseValue` | **T** | The value that is used to drive `TargetField` when `State` is false. |
| `TrueValue` | **T** | The value that is used to drive `TargetField` when `State` is true. |

Fields
Collapse

## Usage

`TargetField` is the field to drive, and has the same type as specified during component creation. When `State` is false, the field pointed to by `TargetField` will take the value of `FalseValue`. When it is true, the field will take the value of `TrueValue`.

## Examples

One popular use of this component is to provide a way to control a blendshape that needs floats from a toggle that is typically a bool. The flexibility of this component also allows for both inverting a '1 when Off' type blendshape into 'on when true' bool, as well as when driving blendshapes that don't need to be driven to 1, for example if a blendshape controls the size of an ear and 0.5 is the 'on' it allows toggling between 0 and 0.5.

## See Also

- [ProtoFlux:Conditional](https://wiki.resonite.com/ProtoFlux:Conditional "ProtoFlux:Conditional")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BooleanValueDriver&oldid=113547](https://wiki.resonite.com/index.php?title=Component:BooleanValueDriver&oldid=113547)"

Contents