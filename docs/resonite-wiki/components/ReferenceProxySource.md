# Component:ReferenceProxySource

> Source: https://wiki.resonite.com/Component:ReferenceProxySource

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ReferenceProxySource&diff=88799) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2d/ReferenceProxySourceComponent.png/510px-ReferenceProxySourceComponent.png)](https://wiki.resonite.com/File:ReferenceProxySourceComponent.png) **ReferenceProxySource** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ReferenceProxySource** component allows for the [user](https://wiki.resonite.com/User "User") to grab a [reference](https://wiki.resonite.com/Reference_Type "Reference Type") off from a [UIX](https://wiki.resonite.com/UIX "UIX") element. This requires a [Button](https://wiki.resonite.com/Component:Button "Component:Button") component to work.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Reference` | _direct_ **[SyncRef](https://wiki.resonite.com/Type:SyncRef "Type:SyncRef")** | The reference itself. |

Fields
Collapse

## Usage

This is used to carry references to other fields that are looking for it. Using this component along with the [ReferenceGrabReceiver](https://wiki.resonite.com/Component:ReferenceGrabReceiver "Component:ReferenceGrabReceiver") and [ReferenceField](https://wiki.resonite.com/Component:ReferenceField "Component:ReferenceField") of the type [IWorldElement](https://wiki.resonite.com/Type:IWorldElement "Type:IWorldElement") will allow the user to carry the [reference](https://wiki.resonite.com/Reference_Type "Reference Type") from source to receiver directly.

## Examples

## See Also

- Similar to the [ValueFieldProxySource](https://wiki.resonite.com/Component:ValueFieldProxySource "Component:ValueFieldProxySource") and [ValueProxySource](https://wiki.resonite.com/Component:ValueProxySource "Component:ValueProxySource") components.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceProxySource&oldid=88799](https://wiki.resonite.com/index.php?title=Component:ReferenceProxySource&oldid=88799)"

Contents