# Component:LegacyWorldThumbnailItem

> Source: https://wiki.resonite.com/Component:LegacyWorldThumbnailItem

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/61/WorldThumbnailItemComponent.png/510px-WorldThumbnailItemComponent.png)](https://wiki.resonite.com/File:WorldThumbnailItemComponent.png) **Legacy World Thumbnail Item** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyWorldThumbnailItem** component is used to show worlds in the list of the legacy world facet.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UpdatingUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user managing updating this component's functionality. |
| `WorldOrSessionId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The world or session ID this component is providing information on. |
| `_visited` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the World has been visited by `UpdatingUser`. |
| `_totalActiveUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The total focused and active users in the world. |
| `_totalContacts` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The total amount of users on the world that are contacts of `UpdatingUser`. |
| `PressAction` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[LegacyWorldItemAction](https://wiki.resonite.com/index.php?title=Type:LegacyWorldItemAction&action=edit&redlink=1 "Type:LegacyWorldItemAction (page does not exist)")** | The action to preform when clicking on this item. |
| `_thumbnailGraphic` | **[RawGraphic](https://wiki.resonite.com/Component:RawGraphic "Component:RawGraphic")** | The component handling the Thumbnail graphic. |
| `_thumbnailTexture` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The component handling the Thumbnail texture. |
| `_nameRoot` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The component that is the graphic rectangle handler for the world name. |
| `_detailRoot` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The component that is the graphic rectangle handler for the world details. |
| `_visitedRoot` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The component that is the graphic rectangle handler for the world visited status. |
| `_counterRoot` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The component that is the graphic rectangle handler for the world active users and contacts amount. |
| `_iconsRoot` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The component that is the graphic rectangle handler for the world icons. |
| `_closeButton` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The component that is the graphic rectangle handler for the world close button. |
| `_nameText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text showing the world name. |
| `_detailText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text showing the world details. |
| `_counterText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text showing the world active user/contacts. |
| `_borderOverlay` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The image UIX component handling the border graphic |
| `_borderColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the border should be. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnClose:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the close button is touched. |

Triggers
Collapse

## Usage

Don't use.

## Examples

Used in the old legacy world browser.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyWorldThumbnailItem&oldid=99062](https://wiki.resonite.com/index.php?title=Component:LegacyWorldThumbnailItem&oldid=99062)"

Contents