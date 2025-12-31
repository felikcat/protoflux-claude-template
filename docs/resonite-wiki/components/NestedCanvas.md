# Component:NestedCanvas

> Source: https://wiki.resonite.com/Component:NestedCanvas

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:NestedCanvas&diff=96233) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/cf/NestedCanvasComponent.png/510px-NestedCanvasComponent.png)](https://wiki.resonite.com/File:NestedCanvasComponent.png) **NestedCanvas** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Nested Canvas** component takes in a target [Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas") to nest as, and then it drives the values to the `StartingOffset`, `StartingMaskDepth`, and sets the [BoxCollider](https://wiki.resonite.com/Component:BoxCollider "Component:BoxCollider")`Offset` and `Size`, for consistency with the main canvas this component is under.

This is essentially a component that can nest (or you can think of it as masking) another uix canvas within another canvas, this can be transformed to your liking, which makes it very useful for rotating UIX. Interactions are also communicated as well.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetCanvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The target canvas to nest as |
| `_renderOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The render offset reference from the target canvas to be applied to the new nested canvas |
| `_maskDepth` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The mask depth reference from the target canvas to be applied to the new nested canvas |

Fields
Collapse

## Usage

This component is used mainly for consistency with other canvas components, no matter where in the world hierarchy. It does not need to be on the same canvas or panel to work.

## Examples

## Related Components

This needs a [Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas") component to work.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NestedCanvas&oldid=96233](https://wiki.resonite.com/index.php?title=Component:NestedCanvas&oldid=96233)"

Contents