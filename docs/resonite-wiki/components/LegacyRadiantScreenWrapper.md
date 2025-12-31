# Component:LegacyRadiantScreenWrapper

> Source: https://wiki.resonite.com/Component:LegacyRadiantScreenWrapper

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[File:LegacyRadiantScreenWrapper\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LegacyRadiantScreenWrapper%601Component.png "File:LegacyRadiantScreenWrapper`1Component.png") **Legacy Radiant Screen Wrapper\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyRadiantScreenWrapper** component was used to handle the old ui when the bottom buttons used to be physical. this should never be used in new content ever.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Icon` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The icon of the current screen. |
| `ActiveColor` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The color of the current screen. |
| `Label` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The label text of the current screen. |
| `ScreenEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled status of the current screen. |
| `BaseResolution` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The base resolution of the current screen. |
| `_screenRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the current screen. |
| `_screenCanvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas component of the current screen. |
| `_modalOverlayManager` | **[ModalOverlayManager](https://wiki.resonite.com/Component:ModalOverlayManager "Component:ModalOverlayManager")** | The modal overlay manager of the dash this component controls. |
| `_button` | **[RadiantDashButton](https://wiki.resonite.com/Component:RadiantDashButton "Component:RadiantDashButton")** | The button for the current screen. |
| `_iconTexture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The icon for the current screen. |
| `ExtraSidePadding` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to pad the current screen |
| `Background` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The background color of the current screen. |
| `_initialized` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component is finished setup. |
| `InitializeComponent` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") <T>** | A sync delegate to call with an argument of **T** when this initalizes. |
| `ButtonGenerated` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [RadiantDashButton](https://wiki.resonite.com/Component:RadiantDashButton "Component:RadiantDashButton") >** | A sync delegate to call with an argument of [RadiantDashButton](https://wiki.resonite.com/Component:RadiantDashButton "Component:RadiantDashButton") to call when this component's button is generated. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyRadiantScreenWrapper&oldid=99050](https://wiki.resonite.com/index.php?title=Component:LegacyRadiantScreenWrapper&oldid=99050)"

Contents