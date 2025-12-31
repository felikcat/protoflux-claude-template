# Component:Snapper

> Source: https://wiki.resonite.com/Component:Snapper

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/ce/SnapperComponent.png/510px-SnapperComponent.png)](https://wiki.resonite.com/File:SnapperComponent.png) **Snapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The Snapper component allows a slot to parent to [Snap Target](https://wiki.resonite.com/Component:SnapTarget "Component:SnapTarget") slots.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UseBoundingBoxCenter` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | _This article or section is a stub. You can help the Resonite wiki by expanding it._ |
| `SnapCheckRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | _This article or section is a stub. You can help the Resonite wiki by expanding it._ |
| `CheckStaticColliders` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allows the [Snapper](https://wiki.resonite.com/Snapper_(Component) "Snapper (Component)") to look for colliders that are set to Static rather then Trigger. |
| `SnapTargetWhitelist` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[SnapTarget](https://wiki.resonite.com/Component:SnapTarget "Component:SnapTarget")** | List of [Snap Targets](https://wiki.resonite.com/SnapTarget_(Component) "SnapTarget (Component)") that the slot can attach to |
| `Keywords` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | List of keywords to match against a corresponding [Snap Targets](https://wiki.resonite.com/SnapTarget_(Component) "SnapTarget (Component)"). Can have multiple keywords to snap to multiple [Snap Targets](https://wiki.resonite.com/SnapTarget_(Component) "SnapTarget (Component)") |

Fields
Collapse

## Behavior

Allows the slot in which this component resides in to snap to a [Snap Target](https://wiki.resonite.com/SnapTarget_(Component) "SnapTarget (Component)") in another slot. The SnapTargetWhitelist allows you to specify a list of SnapTargets that this component will link to in case you want to limit its snapability. The keywords list allows you to provide a list of words which the [Snap Target](https://wiki.resonite.com/SnapTarget_(Component) "SnapTarget (Component)") can use to filter for specific types of snappers.

It is important to have this in a slot shared with a [Grabbable](https://wiki.resonite.com/Grabbable_(Component) "Grabbable (Component)") component in the root link of the object you wish to snap. Snapped components will become children of the snap target.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Snapper&oldid=81821](https://wiki.resonite.com/index.php?title=Component:Snapper&oldid=81821)"

Contents