# Component:ReferenceField

> Source: https://wiki.resonite.com/Component:ReferenceField

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ReferenceField&diff=95253) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/19/ReferenceField%601Component.png/510px-ReferenceField%601Component.png)](https://wiki.resonite.com/File:ReferenceField%601Component.png) **Reference Field** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Reference Field is a component that is able to store a reference for later use, as long as the reference still exists by then.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Reference` | **T** | A field that can be used to store any reference [type](https://wiki.resonite.com/Category:Type "Category:Type"). |

Fields
Collapse

## Usage

This can be used in tandem with a [Reference Grab Receiver Component](https://wiki.resonite.com/Component:ReferenceGrabReceiver "Component:ReferenceGrabReceiver") as a place to store the value received by said component. This component's `Reference` field can be accessed with ProtoFlux.

Using this as a [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") is considered bad practice due to it making your code harder to read, use, and transfer.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ValueField\`1](https://wiki.resonite.com/Component:ValueField%601 "Component:ValueField`1")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceField&oldid=95253](https://wiki.resonite.com/index.php?title=Component:ReferenceField&oldid=95253)"

Contents