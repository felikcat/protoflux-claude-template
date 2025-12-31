# Component:SnapTarget

> Source: https://wiki.resonite.com/Component:SnapTarget

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/01/SnapTargetComponent.png/510px-SnapTargetComponent.png)](https://wiki.resonite.com/File:SnapTargetComponent.png) **SnapTarget** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SnapTarget** component allows a slot with a [Snapper Component](https://wiki.resonite.com/Snapper_(Component) "Snapper (Component)") to attach to this [slot](https://wiki.resonite.com/Slot "Slot").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SnapperWhitelist` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Snapper](https://wiki.resonite.com/Component:Snapper "Component:Snapper")** | List of [Snappers](https://wiki.resonite.com/Snapper_(Component) "Snapper (Component)") that are allowed to attach to this component |
| `SnapperKeywordWhitelist` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | List of keywords to match against a corresponding [Snapper](https://wiki.resonite.com/Snapper_(Component) "Snapper (Component)") |
| `Filters` | _[list](https://wiki.resonite.com/Type:SyncDelegateList%601 "Type:SyncDelegateList`1")_ of **[SnapperFilter](https://wiki.resonite.com/index.php?title=Type:SnapperFilter&action=edit&redlink=1 "Type:SnapperFilter (page does not exist)")** | _This article or section is a stub. You can help the Resonite wiki by expanding it._ |
| `DirectSnapOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | _Unused_ |
| `MaximumSnapDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum distance the [Snapper](https://wiki.resonite.com/Snapper_(Component) "Snapper (Component)") can snap with the Target. This value drives the [SphereCollider](https://wiki.resonite.com/SphereCollider_(Component) "SphereCollider (Component)") radius |
| `MaximumAngleDeviation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | _This article or section is a stub. You can help the Resonite wiki by expanding it._ |
| `AnimationTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The time it takes for the [Snapper](https://wiki.resonite.com/Snapper_(Component) "Snapper (Component)") to lerp to the Target |
| `AutoSnap` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | _This article or section is a stub. You can help the Resonite wiki by expanding it._ |
| `_snapColliderRadius` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius drive reference of the [SphereCollider](https://wiki.resonite.com/SphereCollider_(Component) "SphereCollider (Component)") |
| `proxySphere` | **[SphereCollider](https://wiki.resonite.com/Component:SphereCollider "Component:SphereCollider")** | Reference of the [SphereCollider](https://wiki.resonite.com/SphereCollider_(Component) "SphereCollider (Component)") that is added on adding the [SnapTarget](https://wiki.resonite.com/SnapTarget_(Component) "SnapTarget (Component)") to a slot |

Fields
Collapse

## Behavior

Allows the slot containing this component to receive slots that contain a [Snapper](https://wiki.resonite.com/Component:Snapper "Component:Snapper") component, the Snapper slot will enter the hierarchy of the SnapTarget slot and get positioned to the center. The SnapperWhitelist allows you to reference specific snappers that you want to allow to link with the SnapTarget. The SnapperKeywordWhitelist allows Snappers with the same keyword to link with the SnapTarget.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SnapTarget&oldid=81823](https://wiki.resonite.com/index.php?title=Component:SnapTarget&oldid=81823)"

Contents