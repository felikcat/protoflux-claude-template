# Component:HyperlinkOpenDialog

> Source: https://wiki.resonite.com/Component:HyperlinkOpenDialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:HyperlinkOpenDialogComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=HyperlinkOpenDialogComponent.png "File:HyperlinkOpenDialogComponent.png") **Hyperlink Open Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **HyperlinkOpenDialog** component shows in user space as a UIX when the user clicks on a [HyperLink](https://wiki.resonite.com/Component:Hyperlink "Component:Hyperlink") component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The url being accessed. |
| `_hyperlinkText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to fill with what is being accessed. |
| `_reasonText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to show the reason for the link dialog showing. |
| `_openButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to open the link in `URL` using the user's OS default browser. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Cancel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Cancel and don't open the link. |
| `Open:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Open the requested link. |

Triggers
Collapse

## Usage

Not used directly by the user.

## Examples

The grant access dialogue when clicking on a link.

## See Also

- [Component:Hyperlink](https://wiki.resonite.com/Component:Hyperlink "Component:Hyperlink")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HyperlinkOpenDialog&oldid=98816](https://wiki.resonite.com/index.php?title=Component:HyperlinkOpenDialog&oldid=98816)"

Contents