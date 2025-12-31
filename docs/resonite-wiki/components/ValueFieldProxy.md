# Component:ValueFieldProxy

> Source: https://wiki.resonite.com/Component:ValueFieldProxy

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3f/ValueFieldProxy%601Component.png/510px-ValueFieldProxy%601Component.png)](https://wiki.resonite.com/File:ValueFieldProxy%601Component.png) **Value Field Proxy\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Value Field Proxy** component is used to make a field accessible via grabbing when paired with a grabbable. See [#Usage](https://wiki.resonite.com/Component:ValueFieldProxy#Usage) for more info.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>** | The field to relay into the grabbable behavior this component has when paired with a grabbable. |

Fields
Collapse

## Usage

Used to make a grabbable object able to put a value into a field. This can be done by clicking with or letting go of the object while holding it and pointing at a collider that can recieve it. Examples of recievers include inspector fields, text fields, and number fields. These objects achieve this by using a [ValueReceiver](https://wiki.resonite.com/Component:ValueReceiver "Component:ValueReceiver").

## Examples

The grabbable behavior of inspector values that allow grabbing values and dropping them into other inspectors. Known as proxy UIs, they also use this component.

## See Also

- [Component:ValueReceiver](https://wiki.resonite.com/Component:ValueReceiver "Component:ValueReceiver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueFieldProxy&oldid=102960](https://wiki.resonite.com/index.php?title=Component:ValueFieldProxy&oldid=102960)"

Contents