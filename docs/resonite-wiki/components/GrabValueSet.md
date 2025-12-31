# Component:GrabValueSet

> Source: https://wiki.resonite.com/Component:GrabValueSet

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/61/GrabValueSet%601Component.png/510px-GrabValueSet%601Component.png)](https://wiki.resonite.com/File:GrabValueSet%601Component.png) **Grab Value Set\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GrabValueSet** component has options to set the value within a value field upon release and/or grabbing of a grabbable Component on the same slot.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>** | The field to set the contained value of during grabbing events. |
| `GrabbedValue` | **T** | The value to set the contained data of the Field referenced in `Target` when the item is grabbed. |
| `ReleasedValue` | **T** | The value to set the contained data of the Field referenced in `Target` when the item is let go of. |
| `SetOnGrabbed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set the contained value of the field referenced by `Target` on grabbed. |
| `SetOnReleased` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set the contained value of the field referenced by `Target` on letting go. |

Fields
Collapse

## Usage

Can be used to change the color of an item on grab or release, or any other value type.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:GrabReferenceSet](https://wiki.resonite.com/Component:GrabReferenceSet "Component:GrabReferenceSet")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabValueSet&oldid=94780](https://wiki.resonite.com/index.php?title=Component:GrabValueSet&oldid=94780)"

Contents