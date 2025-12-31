# Component:UpdateTransform

> Source: https://wiki.resonite.com/Component:UpdateTransform

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5c/UpdateTransformComponent.png/510px-UpdateTransformComponent.png)](https://wiki.resonite.com/File:UpdateTransformComponent.png) **Update Transform** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Update transform is part of the [Undo](https://wiki.resonite.com/Undo "Undo") system, and is used in the [Undo Manager](https://wiki.resonite.com/Component:UndoManager "Component:UndoManager") to allow undoing and redoing of moving an object.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that was moved. |
| `RestoreParent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to restore the parent object. |
| `RestorePosition` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to restore the position of the object. |
| `RestoreRotation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to restore the rotation of the object. |
| `RestoreScale` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to restore the scale of the object. |
| `ParentBefore` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The parent slot that the object had before the move. |
| `ParentAfter` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The parent slot the object had after the move. |
| `LocalPositionBefore` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The Local Position that the object had before the move. |
| `LocalRotationBefore` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The Local Rotation that the object had before the move. |
| `LocalScaleBefore` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The Local Scale that the object had before the move. |
| `GlobalPositionBefore` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The Global Position that the object had before the move. |
| `GlobalRotationBefore` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The Global Rotation that the object had before the move. |
| `GlobalScaleBefore` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The Global Scale that the object had before the move. |
| `LocalPositionAfter` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The Local Position the object had after the move. |
| `LocalRotationAfter` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The Local Rotation the object had after the move. |
| `LocalScaleAfter` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The Local Scale the object had after the move. |
| `GlobalPositionAfter` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The Global Position the object had after the move. |
| `GlobalRotationAfter` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The Global Rotation the object had after the move. |
| `GlobalScaleAfter` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The Global Scale the object had after the move. |
| `_performed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the action is performed or it is in the future (due to undoing by the user. |
| `_description` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The description of this move action. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UpdateTransform&oldid=106605](https://wiki.resonite.com/index.php?title=Component:UpdateTransform&oldid=106605)"

Contents