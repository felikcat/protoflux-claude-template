# Component:ValueFieldProxySource

> Source: https://wiki.resonite.com/Component:ValueFieldProxySource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/43/ValueFieldProxySource%601Component.png/510px-ValueFieldProxySource%601Component.png)](https://wiki.resonite.com/File:ValueFieldProxySource%601Component.png) **Value Field Proxy Source\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueFieldProxySource** component allows for the [user](https://wiki.resonite.com/User "User") to grab a value from what is stored in a field off from a [UIX](https://wiki.resonite.com/UIX "UIX") element. This requires a [Button](https://wiki.resonite.com/Component:Button "Component:Button") component to work.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Field` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>** | The field to grab a value from. |

Fields
Collapse

## Usage

This is used to carry values to other [UIX](https://wiki.resonite.com/UIX "UIX") elements that are looking for it. Using this component along with the [ValueReceiver](https://wiki.resonite.com/Component:ValueReceiver "Component:ValueReceiver") and [ValueField](https://wiki.resonite.com/Component:ValueField "Component:ValueField") will allow the user to carry the field's value from source to receiver directly.

## Examples

## See Also

- Similar to the [ReferenceProxySource](https://wiki.resonite.com/Component:ReferenceProxySource "Component:ReferenceProxySource") and [ValueProxySource](https://wiki.resonite.com/Component:ValueProxySource "Component:ValueProxySource") components.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueFieldProxySource&oldid=96464](https://wiki.resonite.com/index.php?title=Component:ValueFieldProxySource&oldid=96464)"

Contents