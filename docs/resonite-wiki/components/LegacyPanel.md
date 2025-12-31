# Component:LegacyPanel

> Source: https://wiki.resonite.com/Component:LegacyPanel

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/00/LegacyPanelComponent.png/510px-LegacyPanelComponent.png)](https://wiki.resonite.com/File:LegacyPanelComponent.png) **Legacy Panel** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyPanel** component is used in old migrated legacy content UI.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Style` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle") >** | The style that determines what this panel looks like. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `ShowHeader` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the panel title. |
| `ShowHandle` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show the panel side bar bevel mesh. |
| `Padding` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much padding should be used from the edge to the inner content. |
| `ZPadding` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much the UI elements should float above the backing plate. |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The thickness of the beveled panel mesh. |
| `WhiteList` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IBounded](https://wiki.resonite.com/Type:IBounded "Type:IBounded")** | Elements that should not be used in the bounds calculations. |
| `BlackList` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IBounded](https://wiki.resonite.com/Type:IBounded "Type:IBounded")** | Elements that should be used in the bounds calculations. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the panel. |
| `_material` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material being used for this panel. |
| `_panelMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelPlaneMesh](https://wiki.resonite.com/Component:BevelPlaneMesh "Component:BevelPlaneMesh")** | The mesh being used for this panel. |
| `_panelPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of this panel. |
| `_handleActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The handle active field of this panel. |
| `_headerActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The header active field of this panel. |
| `_handleMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The handle mesh of this panel. |
| `_handlePos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The handle position of this panel. |
| `_handleColliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The handle collider size of this panel. |
| `_headerTitleMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The title mesh of this panel. |
| `_headerButtonMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BevelStripeMesh](https://wiki.resonite.com/Component:BevelStripeMesh "Component:BevelStripeMesh")** | The header button mesh of this panel. |
| `_headerCollider` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The header collider of this panel. |
| `_headerPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The header position field of this panel. |
| `_headerTitlePos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The header title position of this panel. |
| `_title` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The title name of this panel. |
| `_titleText` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer that displays the title of this panel. |
| `_indicatePrivate` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Is used to change the colors of the panel to indicate that it is in [userspace](https://wiki.resonite.com/Userspace "Userspace"). |
| `_titlePos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the title of this panel |
| `_titleBounds` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The bounds of the title of this panel. |
| `_contentSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The content root slot of this panel. |
| `_headerRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The header root slot of this panel. |
| `_handleAnchorPoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The side bar handle mesh's anchor point for this panel. |
| `_handleAnchorPointPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The handle position field of this panel. |
| `_userspaceOwner` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The owner of this panel. |
| `_titleButtons` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LegacyPanel.TitleButton](https://wiki.resonite.com/Component:LegacyPanel#TitleButton)** | The list of buttons that make up the panel's title. |
| `_highlightedButton` | **[LegacyPanel.TitleButton](https://wiki.resonite.com/Component:LegacyPanel#TitleButton)** | The title button object for the currently highlighted button. |
| `_pinButton` | **[LegacyPanel.TitleButton](https://wiki.resonite.com/Component:LegacyPanel#TitleButton)** | The title button object for the pin to user button. |
| `CloseOverride` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <LegacyPanel>** | A sync delegate that takes a LegacyPanel that overrides the handling of closing this panel. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `HeaderButtonTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the header button is touched. |
| ``OnClose:Action`1<LegacyPanel.TitleButton>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacyPanel.TitleButton](https://wiki.resonite.com/Component:LegacyPanel#TitleButton) >** | ✓ | Called when the panel is closed. |
| ``OnHide:Action`1<LegacyPanel.TitleButton>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacyPanel.TitleButton](https://wiki.resonite.com/Component:LegacyPanel#TitleButton) >** | ✓ | Called when the panel is hidden by the user. |
| ``OnParent:Action`1<LegacyPanel.TitleButton>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacyPanel.TitleButton](https://wiki.resonite.com/Component:LegacyPanel#TitleButton) >** | ✓ | Called when the panel is pinned to the user via the pin button. |
| ``OnUserspaceTransfer:Action`1<LegacyPanel.TitleButton>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacyPanel.TitleButton](https://wiki.resonite.com/Component:LegacyPanel#TitleButton) >** | ✓ | Called when the panel is transfered from [userspace](https://wiki.resonite.com/Userspace "Userspace") to the currently focused world. |

Triggers
Collapse

## TitleButton

| Name | Type | Description |
| --- | --- | --- |
| `ItemColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the button item |
| `Pressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[LegacyPanel.TitleButton](https://wiki.resonite.com/Component:LegacyPanel#TitleButton)** | The sync delegate to call when this button is pressed. |
| `Enabled` | **[bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the button is enabled. |
| `_material` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/Component:PBS_RimMetallic "Component:PBS RimMetallic")** | The material of the button. |
| `_iconMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | The icon's material for the button. |
| `_iconTexture` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The icon's texture for the button. |
| `_lastPress` | **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | The last time the button was pressed. |
| `_itemRoot` | _direct_ **[CleanupRef\`1](https://wiki.resonite.com/Type:CleanupRef%601 "Type:CleanupRef`1") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | The button's root hierarchy. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field of the button. |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The collider size field of the button. |
| `_iconSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The icon size field of the button. |
| `_iconOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The icon offset field of the button. |

Fields

## Usage

Don't use in new content.

## Examples

Found in migrated legacy content.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyPanel&oldid=100032](https://wiki.resonite.com/index.php?title=Component:LegacyPanel&oldid=100032)"

Contents