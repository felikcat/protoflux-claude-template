# Component:GrabReferenceSet

> Source: https://wiki.resonite.com/Component:GrabReferenceSet

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/cf/GrabReferenceSet%601Component.png/510px-GrabReferenceSet%601Component.png)](https://wiki.resonite.com/File:GrabReferenceSet%601Component.png) **Grab Reference Set\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GrabReferenceSet** can be used to write a reference to a field on grab and release.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>** | The field in which to change on grab and release. |
| `GrabbedTarget` | **T** | The value to set the contained data of the SyncRef referenced in `Target` when the item is grabbed. |
| `ReleasedTarget` | **T** | The value to set the contained data of the SyncRef referenced in `Target` when the item is released. |
| `SetOnGrabbed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set the contained data of the SyncRef referenced in `Target` when the item is grabbed. |
| `SetOnReleased` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set the contained data of the SyncRef referenced in `Target` when the item is released. |

Fields
Collapse

## Usage

While on the same slot as a Grabbable the component can be configured to set a reference on grabbed and on released.

## Examples

## See Also

- [Component:GrabValueSet](https://wiki.resonite.com/Component:GrabValueSet "Component:GrabValueSet")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabReferenceSet&oldid=94779](https://wiki.resonite.com/index.php?title=Component:GrabReferenceSet&oldid=94779)"

Contents