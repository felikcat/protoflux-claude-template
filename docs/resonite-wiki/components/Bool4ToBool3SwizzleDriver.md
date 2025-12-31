# Component:Bool4ToBool3SwizzleDriver

> Source: https://wiki.resonite.com/Component:Bool4ToBool3SwizzleDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bd/Bool4ToBool3SwizzleDriverComponent.png/510px-Bool4ToBool3SwizzleDriverComponent.png)](https://wiki.resonite.com/File:Bool4ToBool3SwizzleDriverComponent.png) **Bool 4To Bool 3Swizzle Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Swizzle drivers are a type of component that allow for taking the components of a packed value (packed 3 or 4s) and rearrange them into the output. The different packed channels are numbered 0->2 for pack 3's and 0->3 for pack 4's. When driving the output, you have a choice of taking any channel within the pack 3 or 4 by number and driving an output channel with said source number. This can be used to flip axes, zero them out by using -1 as a source channel, or rearrange them. For example, making a 3d point move only on the y axis position of another point (-1, 1, -1).

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool4](https://wiki.resonite.com/Type:Bool4 "Type:Bool4") >>** | The field which to take values from it's components and drive `Target`'s components with them. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool3](https://wiki.resonite.com/Type:Bool3 "Type:Bool3")** | The field which to drive the components of. |
| `X` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Takes the n'th component from `Source` and drives the X component of `Target` with it. |
| `Y` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Takes the n'th component from `Source` and drives the Y component of `Target` with it. |
| `Z` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Takes the n'th component from `Source` and drives the Z component of `Target` with it. |

Fields
Collapse

## Behavior

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Bool4ToBool3SwizzleDriver&oldid=91128](https://wiki.resonite.com/index.php?title=Component:Bool4ToBool3SwizzleDriver&oldid=91128)"

Contents