# Component:LegacyWorldDetail

> Source: https://wiki.resonite.com/Component:LegacyWorldDetail

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0a/WorldDetailComponent.png/510px-WorldDetailComponent.png)](https://wiki.resonite.com/File:WorldDetailComponent.png) **World Detail** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldDetail** component is used to display information about a world to a UI.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UpdatingUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user managing updates for this component. |
| `WorldOrSessionId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The world or session ID to get info on. |
| `_visited` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `UpdatingUser` has visited this world. |
| `_totalActiveUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many active ussrs are in the world. |
| `_totalContacts` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many contacts of `UpdatingUser` are in the world. |
| `Expanded` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the world item UI has been hovered over in the dash. |
| `CompactDetailExpanded` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the extra detail has been expanded. |
| `CompactDetailCategory` | **[LegacyWorldDetail.DetailCategory](https://wiki.resonite.com/Component:LegacyWorldDetail#DetailCategory)** | The detail to show in the compact view. |
| `ModalCompactSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The size of the world item when not hovered over. |
| `ModalExpandedSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The size of the world item when hovered over. |
| `_hostText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The Text Component showing the host name. |
| `_sessionItemsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot containing current sessions of the world. |
| `_thumbnailGraphic` | **[RawGraphic](https://wiki.resonite.com/Component:RawGraphic "Component:RawGraphic")** | The UIX graphic showing the thumbnail. |
| `_thumbnailTexture` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The texture for the world thumbnail. |
| `_detailImageRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the detail image graphic. |
| `_compactRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the graphic when it is not clicked into. |
| `_compactHeaderRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the root of the text graphic of the world item before clicking into it. |
| `_detailHeaderRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the root of the text graphic of the world item after clicking into it. |
| `_compactMaskEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive for whether or not the compact view mask should be enabled. |
| `_compactMaskRootEnabled` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive for whether or not the compact mask root slot should be enabled. |
| `_openButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button Component for opening the world. |
| `_scrollRect` | **[ScrollRect](https://wiki.resonite.com/Component:ScrollRect "Component:ScrollRect")** | The scroll rectangle for the detail menu of the world item. |
| `_expandButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used for showing the un compact view. |
| `_expandIcon` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The icon for `_expandButton`. |
| `_expandSprite` | **[Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite")** | The sprite for `_expandButton`. |
| `_compactSprite` | **[Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite")** | The sprite for the switch to compact mode. |
| `_description` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text used to show the world description. |
| `_leftDetailsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot used to store the left side details. |
| `_rightDetailsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot used to store the right side details. |
| `_detailsText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text used to show the world details. |
| `_cycleLeftButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | the button for cycling left. |
| `_cycleRightButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | the button for cycling right. |
| `_compactParent` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | the parent slot of the compact view graphic. |
| `_compactHeaderParent` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | the parent slot of the compact views text header. |
| `_sidebarActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with whether the sidebar should be active. |
| `_sidebarAnchorMin` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive for the sidebar's rectangle anchor minimum. |
| `_sidebarAnchorMax` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive for the sidebar's rectangle anchor maximum. |
| `_contentAnchorMin` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive for the content's rectangle anchor minimum. |
| `_contentAnchorMax` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive for the content's rectangle anchor maximum. |
| `_rectTransformLerp` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive for the animation transitions for the item hovering. |
| `_modalAnchorMin` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive for the modal's rectangle anchor minimum. |
| `_modalAnchorMax` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive for the modal's rectangle anchor maximum. |
| `_compactButtonsActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive for the compact buttons active status. |
| `_compactButtonsAnchorMin` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive for the compact buttons rectangle anchor minimum. |
| `_compactButtonsAnchorMax` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive for the compact buttons rectangle anchor maximum. |
| `_compactDetailRect` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The field to drive with the current compact details rectangle component. |
| `_compactDetailButtonRect` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The field to drive with the current compact details button rectangle component. |
| `_compactDetailText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text field that stores the compact view details. |
| `_compactDetailExpandButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button Component that is used to expand the details in the compact view. |
| `_newSessionItemRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot for the graphic for making a new session button. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `ToggleExpanded:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the toggle expanded button is touched. |
| `OnOpen:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the open button is touched. |
| `OnCycleLeft:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the cycle left button is touched. |
| `OnCycleRight:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the cycle right button is touched. |
| ``OnSessionSelected:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | Called when the session select button is touched. |
| `OnCancel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the cancel button is touched. |
| `OnGetWorldOrb:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the get world orb button is touched. |
| `OnCopyWorldURL:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the copy world url button is touched. |
| `OnCopyRecordURL:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the copy record url button is touched. |
| `OnStartCustomSession:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the start custom session button is touched. |
| `OnModifyMetadata:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the modify meta data button is touched. |
| ``CustomWorldStart:Action`1<NewWorldDialog>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [NewWorldDialog](https://wiki.resonite.com/Component:NewWorldDialog "Component:NewWorldDialog") >** | ✓ | Called when the start custom session button is touched. |
| `OnGetSessionOrb:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the get session orb button is touched. |
| `OnCopySessionURL:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the copy session url button is touched. |
| ``OnAdminAddTag:ButtonEventHandler`1<TextField>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [TextField](https://wiki.resonite.com/Component:TextField "Component:TextField") >** | ✓ | Called when the add tag button by admins is touched. |
| `OnFeature:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the feature world button is touched. |
| `OnRemoveSubmission:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the remove submission button is touched. |

Triggers
Collapse

## DetailCategory

| Name | Value | Description |
| --- | --- | --- |
| `Users` | 0 | Show the users. |
| `Description` | 1 | Show the description. |

Values

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in the dash previously.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyWorldDetail&oldid=99061](https://wiki.resonite.com/index.php?title=Component:LegacyWorldDetail&oldid=99061)"

Contents