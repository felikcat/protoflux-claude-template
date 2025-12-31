# Component:DesktopDisplayLayout

> Source: https://wiki.resonite.com/Component:DesktopDisplayLayout

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e3/DesktopDisplayLayoutComponent.png/510px-DesktopDisplayLayoutComponent.png)](https://wiki.resonite.com/File:DesktopDisplayLayoutComponent.png) **DesktopDisplayLayout** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DesktopDisplayLayout** component displays a list of display selection buttons for a user's monitor settup. It is used in the [dash menu](https://wiki.resonite.com/Dash_menu "Dash menu") and only works in [userspace](https://wiki.resonite.com/Userspace "Userspace").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `User` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user to get displays for. |
| `DisplayTemplate` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the template to use when generating display selection buttons. |
| `ItemGenerated` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[DesktopDisplayLayout.DisplayItemHandler](https://wiki.resonite.com/Component:DesktopDisplayLayout#DisplayItemHandler)** | usually the OnDisplayItemGenerated() sync delegate from [DesktopControlDialog](https://wiki.resonite.com/Component:DesktopControlDialog#Sync_Delegates "Component:DesktopControlDialog"). |

Fields
Collapse

## DisplayItemHandler

A Sync delegate of type [Delegate](https://wiki.resonite.com/Type:Delegate "Type:Delegate") < [Display](https://wiki.resonite.com/index.php?title=Type:Display&action=edit&redlink=1 "Type:Display (page does not exist)") display, [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") itemRoot>

## Examples

Used in the dash desktop tab.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DesktopDisplayLayout&oldid=100116](https://wiki.resonite.com/index.php?title=Component:DesktopDisplayLayout&oldid=100116)"

Contents