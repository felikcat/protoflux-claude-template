# Component:LegacyHorizontalChoiceBar

> Source: https://wiki.resonite.com/Component:LegacyHorizontalChoiceBar

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/55/LegacyHorizontalChoiceBarComponent.png/510px-LegacyHorizontalChoiceBarComponent.png)](https://wiki.resonite.com/File:LegacyHorizontalChoiceBarComponent.png) **Legacy Horizontal Choice Bar** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyHorizontalChoiceBar** component is used in old migrated legacy content. This should not be used in new content, and should be replaced whenever possible. This was primarily used in old Gizmos.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Style` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle") >** | The source of the legacy color styles for this component. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `_items` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LegacyHorizontalChoiceBar.Item](https://wiki.resonite.com/Component:LegacyHorizontalChoiceBar#Item)** | A list of items to be able to press. |
| `Width` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width of each item. |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of each item. |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of each item. |
| `Spacing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far apart the items should be placed. |
| `Slant` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The Bevel of the meshes of each item. |
| `Symmetrical` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the Horizontal layout should be symmetrical. |
| `SegmentTouched` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[LegacyHorizontalChoiceBar.SegmentTouchEvent](https://wiki.resonite.com/Component:LegacyHorizontalChoiceBar#SegmentTouchEvent)** | The Sync delegate to call whenever an item is touched. |
| `_root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the place to parent all the items. |
| `_rootScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of the slot to place the items. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnSegmentTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called whenever a segment is touched. |

Triggers
Collapse

## Item

| Name | Type | Description |
| --- | --- | --- |
| `OverrideColor` | **[colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use for this item rather than the one the root Component uses. |
| `Highlight` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this item should be highlighted. |
| `Touched` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | The Sync delegate to call when this item is touched. |
| `_slot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of this item option. |
| `_text` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer") >** | The text of this item option. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the slot of this item. |
| `_textPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the text of this item. |
| `_textBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The text bounds field. |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size of this item's collider. |
| `_colliderOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset of this item's collider. |
| `_mesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The mesh of this item. |
| `_material` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/Component:PBS_RimMetallic "Component:PBS RimMetallic")** | The material of the mesh of this item. |

Fields

## SegmentTouchEvent

SegmentTouchEvent() is a sync delegate that is the type [Delegate](https://wiki.resonite.com/Type:Delegate "Type:Delegate") <LegacyHorizontalChoiceBar sender, [Int](https://wiki.resonite.com/Type:Int "Type:Int") itemIndex, [TouchEventInfo](https://wiki.resonite.com/index.php?title=Type:TouchEventInfo&action=edit&redlink=1 "Type:TouchEventInfo (page does not exist)") eventInfo> and can be used to handle the press events of a LegacyHorizontalChoiceBar.

## Usage

Just dont.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyHorizontalChoiceBar&oldid=99020](https://wiki.resonite.com/index.php?title=Component:LegacyHorizontalChoiceBar&oldid=99020)"

Contents