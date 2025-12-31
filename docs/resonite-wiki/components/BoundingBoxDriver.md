# Component:BoundingBoxDriver

> Source: https://wiki.resonite.com/Component:BoundingBoxDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BoundingBoxDriver&diff=93413) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/81/BoundingBoxDriverComponent.png/510px-BoundingBoxDriverComponent.png)](https://wiki.resonite.com/File:BoundingBoxDriverComponent.png) **Bounding Box Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BoundingBoxDriver** component is commonly used in Basic text objects to size the collider based on the text. This takes any [IBounded](https://wiki.resonite.com/Type:IBounded "Type:IBounded") and turns its Bounding box data into its local space center point and local space size. This is useful for auto generating the size and center of a [Component:BoxCollider](https://wiki.resonite.com/Component:BoxCollider "Component:BoxCollider") around a procedural mesh.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BoundedSource` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IBounded](https://wiki.resonite.com/Type:IBounded "Type:IBounded") >** | The object to get Bounding box data from. |
| `Size` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the local space size of the bounding box of `BoundedSource`. |
| `Center` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the local space center of the bounding box of `BoundedSource`. |
| `Padding` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | how much to add to the output of `Size` |
| `Scale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | how much to multiply the output of `Size` |

Fields
Collapse

## Usage

Attach to a slot and provide `BoundedSource`. The output fields are best used to drive a [Component:BoxCollider](https://wiki.resonite.com/Component:BoxCollider "Component:BoxCollider").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:BoxCollider](https://wiki.resonite.com/Component:BoxCollider "Component:BoxCollider")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoundingBoxDriver&oldid=93413](https://wiki.resonite.com/index.php?title=Component:BoundingBoxDriver&oldid=93413)"

Contents