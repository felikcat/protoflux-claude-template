# Component:ReferenceDriveReceiver

> Source: https://wiki.resonite.com/Component:ReferenceDriveReceiver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ab/ReferenceDriveReceiver%601Component.png/510px-ReferenceDriveReceiver%601Component.png)](https://wiki.resonite.com/File:ReferenceDriveReceiver%601Component.png) **Reference Drive Receiver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ReferenceDriveReceiver** component is used to allow dropping a reference proxy via the user's hand onto a UIX element to trigger the prompt for driving a reference field. This requires a UIX button to work.

## Fields.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Reference` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>** | The field this should allow an option to drive for when a reference is dropped onto the UIX element this is on. |

Fields
Collapse

## Usage

Attach to a slot as part of a [Component:Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas") hierarchy with a [Component:Button](https://wiki.resonite.com/Component:Button "Component:Button") in the same slot. Provide a value for `Reference` for it to start working.

## Examples

Used in [Scene Inspectors](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") to allow for driving reference fields by dragging and dropping references.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceDriveReceiver&oldid=106537](https://wiki.resonite.com/index.php?title=Component:ReferenceDriveReceiver&oldid=106537)"

Contents