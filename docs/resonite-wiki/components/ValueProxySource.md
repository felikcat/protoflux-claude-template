# Component:ValueProxySource

> Source: https://wiki.resonite.com/Component:ValueProxySource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/df/ValueProxySource%601Component.png/510px-ValueProxySource%601Component.png)](https://wiki.resonite.com/File:ValueProxySource%601Component.png) **Value Proxy Source\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueProxySource** component allows for the [user](https://wiki.resonite.com/User "User") to grab a [value](https://wiki.resonite.com/Value_Type "Value Type") off from a [UIX](https://wiki.resonite.com/UIX "UIX") element. This requires a [Button](https://wiki.resonite.com/Component:Button "Component:Button") component to work.

![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

**DO NOT** use any other type than a [Value Type](https://wiki.resonite.com/Value_Type "Value Type") when using this component! This component will crash a world with a [Reference Type](https://wiki.resonite.com/Reference_Type "Reference Type")!


| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Value` | **T** | The value itself. |

Fields
Collapse

## Usage

This is used to carry values to other [UIX](https://wiki.resonite.com/UIX "UIX") elements that are looking for it. Using this component along with the [ValueReceiver](https://wiki.resonite.com/Component:ValueReceiver "Component:ValueReceiver") and [ValueField](https://wiki.resonite.com/Component:ValueField "Component:ValueField") of a [value type](https://wiki.resonite.com/Value_Type "Value Type") will allow the user to carry the value from source to receiver directly.

## Examples

## See Also

- Similar to the [ReferenceProxySource](https://wiki.resonite.com/Component:ReferenceProxySource "Component:ReferenceProxySource") and [ValueFieldProxySource](https://wiki.resonite.com/Component:ValueFieldProxySource "Component:ValueFieldProxySource") components.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueProxySource&oldid=96462](https://wiki.resonite.com/index.php?title=Component:ValueProxySource&oldid=96462)"

Contents