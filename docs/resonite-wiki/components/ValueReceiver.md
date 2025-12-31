# Component:ValueReceiver

> Source: https://wiki.resonite.com/Component:ValueReceiver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b1/ValueReceiver%601Component.png/510px-ValueReceiver%601Component.png)](https://wiki.resonite.com/File:ValueReceiver%601Component.png) **Value Receiver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueReceiver** component can receive a value dropped onto a [UIX](https://wiki.resonite.com/UIX "UIX") element [Button](https://wiki.resonite.com/Component:Button "Component:Button") by a [user](https://wiki.resonite.com/User "User"). The value dropped is then stored into the field specified by `Field` (an example would be to use [ValueField](https://wiki.resonite.com/Component:ValueField "Component:ValueField"))

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Field` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>** | The field to store the received value |
| `Undoable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether dropping elements onto this UIX interactable is undoable. |
| `TryConvertValues` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether dropped elements that do not match the type of the receiver are attempted to be converted to the type |

Fields
Collapse

## Behavior

## Examples

## See Also

- [Component:ReferenceReceiver](https://wiki.resonite.com/Component:ReferenceReceiver "Component:ReferenceReceiver")
- [Component:AssetReceiver](https://wiki.resonite.com/Component:AssetReceiver "Component:AssetReceiver")
- [Component:ValueProxy](https://wiki.resonite.com/Component:ValueProxy "Component:ValueProxy")
- [Component:ValueFieldProxy](https://wiki.resonite.com/Component:ValueFieldProxy "Component:ValueFieldProxy")

Retrieved from " [https://wiki.resonite.com/index.php?title=User:Grand/Component:ValueReceiver&oldid=96668](https://wiki.resonite.com/index.php?title=User:Grand/Component:ValueReceiver&oldid=96668)"

Contents