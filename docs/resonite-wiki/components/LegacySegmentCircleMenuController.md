# Component:LegacySegmentCircleMenuController

> Source: https://wiki.resonite.com/Component:LegacySegmentCircleMenuController

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e1/LegacySegmentCircleMenuControllerComponent.png/510px-LegacySegmentCircleMenuControllerComponent.png)](https://wiki.resonite.com/File:LegacySegmentCircleMenuControllerComponent.png) **Legacy Segment Circle Menu Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This is a Legacy item and should not be used.

> From a long dead platform. he who shall not be named on the holy land that is this wiki
>
> — [989onan](https://wiki.resonite.com/User:989onan "User:989onan")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DefaultFontMaterial` | **[TextUnlitMaterial](https://wiki.resonite.com/index.php?title=TextUnlitMaterial&action=edit&redlink=1 "TextUnlitMaterial (page does not exist)")** | The default font to use for menu items. |
| `DisabledOutlineColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The outline color menu items should have when disabled. |
| `DisabledFillColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color menu items should have when disabled. |
| `LogoCircle` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this is a logo Circle from a long dead platform. he who shall not be named on the holy land that is this wiki - [@989onan](https://wiki.resonite.com/User:989onan "User:989onan"). |
| `GenerateColliders` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to generate colliders for menu items. |
| `HighlightRadiusOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The tolerance for highlighting menu items. |
| `logoMenuMesh` | **[LegacyCircleSegmentMesh](https://wiki.resonite.com/Component:LegacyCircleSegmentMesh "Component:LegacyCircleSegmentMesh")** | The logo mesh from a long dead platform. he who shall not be named on the holy land that is this wiki - [@989onan](https://wiki.resonite.com/User:989onan "User:989onan"). |
| `circleMenuItems` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item)** | The list of menu items this component is managing. |
| `independentMenuItems` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LegacySegmentCircleMenuController.Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item)** | The list of independent menu items this list is managing for other tools. |
| `itemsArcs` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LegacySegmentCircleMenuController.ItemsArc](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#ItemsArc)** | The list of item arcs this component is managing. |
| `_overridesDrive` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncList\`1](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1") < [LegacyCircleSegmentMesh.MenuSegment](https://wiki.resonite.com/Component:LegacyCircleSegmentMesh#MenuSegment "Component:LegacyCircleSegmentMesh") >** | List of menu segments to use as overrides. |
| `_independentDrive` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncList\`1](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1") < [LegacyCircleSegmentMesh.MenuSegment](https://wiki.resonite.com/Component:LegacyCircleSegmentMesh#MenuSegment "Component:LegacyCircleSegmentMesh") >** | List of indepent drives of menu segments. |
| `menuItemsSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to generate and place menu items for this component. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `MenuItemTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when a menu item is touched. |

Triggers
Collapse

## Item

| Name | Type | Description |
| --- | --- | --- |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this item's button is enabled. |
| `AngleStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle on the circle where this starts. |
| `RadiusStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The inner radius from the center. |
| `ArcLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much of the circle in degrees this takes up. |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The outer radius minus inner radius. |
| `Label` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text label for this menu item. |
| `LabelColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The label color for this menu item. |
| `OutlineColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The outline color of this Menu item. |
| `FillColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The fill color of this Menu item |
| `Pressed` | _direct_ **[SyncDelegate](https://wiki.resonite.com/index.php?title=Type:SyncDelegate&action=edit&redlink=1 "Type:SyncDelegate (page does not exist)") < [Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item) >>** | The Sync delegate to call and pass this item as the value when this menu item is pressed. |
| `IconMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | The material for this Menu item's icon |
| `IconTexture` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The texture used for this menu item's icon |
| `RotateIcon` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to rotate the icon. |
| `IconRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the icon graphic. |
| `Highlight` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this menu item is highlighted. |
| `IconPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field of the icon's position. |
| `IconRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field of the icon's rotation. |
| `IconScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field of the icon's scale. |
| `ColliderRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the collider for this menu item. |
| `ColliderPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field of the collider's position. |
| `ColliderScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field of the collider's scale. |
| `ColliderRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field of the collider's rotation. |
| `LastPress` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | The last time the button was pressed in world time. |
| `LabelRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot of the label visual. |
| `LabelPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the label visual. |
| `LabelScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field of the label visual. |
| `LabelColorDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color field of the label visual. |

Fields

## ItemsArc

| Name | Type | Description |
| --- | --- | --- |
| `CenterItem` | **[Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item)** | The item to display in the center. |
| `SeparationAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far apart the items should be. |
| `_left` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ArcItem](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#ArcItem)** | all the items to display along the left side. |
| `_right` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ArcItem](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#ArcItem)** | all the items to display along the right side. |

Fields

### ArcItem

| Name | Type | Description |
| --- | --- | --- |
| `Item` | **[Item](https://wiki.resonite.com/Component:LegacySegmentCircleMenuController#Item)** | The item this arc item contains. |
| `AngleStartDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the starting position of this Menu item on the arc. |

Fields

## Usage

Just don't.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacySegmentCircleMenuController&oldid=99057](https://wiki.resonite.com/index.php?title=Component:LegacySegmentCircleMenuController&oldid=99057)"

Contents