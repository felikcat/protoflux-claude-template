# Component:SetReference

> Source: https://wiki.resonite.com/Component:SetReference

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/06/SetReference%601Component.png/510px-SetReference%601Component.png)](https://wiki.resonite.com/File:SetReference%601Component.png) **Set Reference\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Set Reference** component is internally used by the [Undo System](https://wiki.resonite.com/Undo "Undo") for setting and reverting a [Reference](https://wiki.resonite.com/Reference "Reference").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>** | The field that was changed. |
| `TargetBefore` | **T** | The reference value before the change. |
| `TargetAfter` | **T** | The reference value after the change. |
| `_performed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the undo step was done or undone. |
| `_description` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The description of the change that was made and what to for the context menu label text when undoing/redoing. |

Fields
Collapse

## Usage

Not used directly by the user.

## Examples

See [Undo](https://wiki.resonite.com/Undo "Undo").

## See Also

- [Undo](https://wiki.resonite.com/Undo "Undo")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SetReference&oldid=100864](https://wiki.resonite.com/index.php?title=Component:SetReference&oldid=100864)"

Contents