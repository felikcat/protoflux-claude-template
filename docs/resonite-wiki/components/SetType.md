# Component:SetType

> Source: https://wiki.resonite.com/Component:SetType

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c2/SetTypeComponent.png/510px-SetTypeComponent.png)](https://wiki.resonite.com/File:SetTypeComponent.png) **Set Type** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Set type is a component that is part of the [undo](https://wiki.resonite.com/Undo "Undo") system. This stores an undo step for setting a type field.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The value field for a type value that was changed. |
| `ValueBefore` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The value it was before edit. |
| `ValueAfter` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The value it became after edit. |
| `_performed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this was done (true) or can be redone (false) |
| `_description` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The description of this undo step for changing a type field. |

Fields
Collapse

## Behavior

## Examples

## See Also

[Undo System](https://wiki.resonite.com/Undo "Undo")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SetType&oldid=91444](https://wiki.resonite.com/index.php?title=Component:SetType&oldid=91444)"

Contents