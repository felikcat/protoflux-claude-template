# Component:UserspaceRadiantDash

> Source: https://wiki.resonite.com/Component:UserspaceRadiantDash

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:UserspaceRadiantDashComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=UserspaceRadiantDashComponent.png "File:UserspaceRadiantDashComponent.png") **Userspace Radiant Dash** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserspaceRadiantDash** is better described on the dedicated page, [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BlockOpenClose` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to block opening and closing of the dash |
| `Freeform` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the dash can be grabbed around in freeform style. |
| `_dash` | **[RadiantDash](https://wiki.resonite.com/Component:RadiantDash "Component:RadiantDash")** | The radiant dash component that handles all the dash like behaviors/ |
| `_dashVisualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot for the visuals of the radiant dash. |
| `_positioner` | **[UserInterfacePositioner](https://wiki.resonite.com/Component:UserInterfacePositioner "Component:UserInterfacePositioner")** | Handles positioning the dash in front of the user while it is in user space. |
| `_modalOverlay` | **[ModalOverlayManager](https://wiki.resonite.com/Component:ModalOverlayManager "Component:ModalOverlayManager")** | Handles managing the different overlays on different screens like the home tab. |
| `_legacyInventoryPanel` | **[LegacyCanvasPanel](https://wiki.resonite.com/Component:LegacyCanvasPanel "Component:LegacyCanvasPanel")** | Legacy. not used in newer versions. From a time before time when UIX didn't exist. |
| `_legacyInventory` | **[InventoryBrowser](https://wiki.resonite.com/Component:InventoryBrowser "Component:InventoryBrowser")** | Legacy. not used in newer versions. From a time before time when UIX didn't exist. |
| `_slider` | **[Slider](https://wiki.resonite.com/Component:Slider "Component:Slider")** | The slider used to move the dash around via grabbing it. |
| `_lookat` | **[LookAt](https://wiki.resonite.com/Component:LookAt "Component:LookAt")** | The lookat component that handles keeping the dash facing the user. |
| `_uiEditModeToggle` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that appears when the user has the ability to turn off UI edit mode after turning it on. |
| `_alwaysOnFacetRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | This slot stores elements of the dash that were made on a facet that are marked as always on. Things that end up here will have a [Always On Facet Module Component](https://wiki.resonite.com/Component:AlwaysOnFacetModule "Component:AlwaysOnFacetModule") so they always stay enabled even when the dash closes. |
| `_screensWorkspace` | **[Workspace](https://wiki.resonite.com/Component:Workspace "Component:Workspace")** | The workspace for screens that should be saved when the user's dash gets saved. helps preserve dash customization between machines. |
| `_topWorkspace` | **[Workspace](https://wiki.resonite.com/Component:Workspace "Component:Workspace")** | The workspace for top area elements that should be saved when the user's dash gets saved. helps preserve dash customization between machines. |
| `_notifications` | **[NotificationPanel](https://wiki.resonite.com/Component:NotificationPanel "Component:NotificationPanel")** | The component that handles notifications for the game for the current session and people coming online. |
| `_notificationsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that contains the entirety of the notifications stack and logic. |
| `_notificationsHolder` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot at which notification elements should appear like users joining and role changing. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``OnModalOverlayRequested:Action`1<ModalOverlayManager>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [ModalOverlayManager](https://wiki.resonite.com/Component:ModalOverlayManager "Component:ModalOverlayManager") >** | ✓ | handles when the modal overlay request action is made. |
| `OnTurnOffEditMode:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user requests to turn off edit mode via the button at the bottom of the dash. |
| ``SetupDefaultTopBar:Action`1<Slot>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | ✓ | Handles when the dash requests a setup of a fresh new dash topbar. |
| ``OnHide:Action`1<LegacyPanel>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacyPanel](https://wiki.resonite.com/Component:LegacyPanel "Component:LegacyPanel") >** | ✓ | Handles hiding of legacy panels on dash elements that still use it. |

Triggers
Collapse

## Usage

See [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu").

## Examples

See [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu").

## See Also

- [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserspaceRadiantDash&oldid=100797](https://wiki.resonite.com/index.php?title=Component:UserspaceRadiantDash&oldid=100797)"

Contents