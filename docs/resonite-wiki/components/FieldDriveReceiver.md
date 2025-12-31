# Component:FieldDriveReceiver

> Source: https://wiki.resonite.com/Component:FieldDriveReceiver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a3/FieldDriveReceiver%601Component.png/510px-FieldDriveReceiver%601Component.png)](https://wiki.resonite.com/File:FieldDriveReceiver%601Component.png) **Field Drive Receiver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FieldDriveReceiver** component is used to handle the dropping of field names onto other field names in order to drive one with the other in inspectors, otherwise known as [Drives](https://wiki.resonite.com/Drives "Drives"). This is used as an interactable [UIX](https://wiki.resonite.com/UIX "UIX") element.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Field` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>** | The field to expose to dropping other field names onto it for driving. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in the Inspector to handle field name driving as explained in [Drives](https://wiki.resonite.com/Drives "Drives")

## See Also

- [Drives](https://wiki.resonite.com/Drives "Drives")
- [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FieldDriveReceiver&oldid=96513](https://wiki.resonite.com/index.php?title=Component:FieldDriveReceiver&oldid=96513)"

Contents