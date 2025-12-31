# Component:Hyperlink

> Source: https://wiki.resonite.com/Component:Hyperlink

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Hyperlink&diff=97951) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/74/Hyperlink_Component.webp/510px-Hyperlink_Component.webp.png)](https://wiki.resonite.com/File:Hyperlink_Component.webp) **Hyperlink** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Hyperlink** component allows you to turn an object with a collider into a clickable link that will prompt the user in [Userspace](https://wiki.resonite.com/Userspace "Userspace") to open the provided link in their default web browser.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This component requires the start to contain `http://`, `ws://`, or something similar at the beginning of the URL, or this component will not prompt for a connection.

Example for connecting to the local host of the device: `http://localhost:5000`

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The hyperlink to open. |
| `OpenOnce` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Prevents the user from clicking on the URL more than once and bringing up multiple confirmation dialouges |
| `Reason` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The reason that the hyperlink is being opened. Displayed to the user when they click it in the security dialog. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``Open:Func`1<Bool>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | X | When called, this function will bring up the confirmation dialogue for the user that is executing the function (local user). |

Triggers
Collapse

## Usage

It can be triggered or activated in the following ways:

- Using a collider and physically touching the object to prompt for a connection.
- Attaching a [UIX](https://wiki.resonite.com/UIX "UIX") [button](https://wiki.resonite.com/Component:Button "Component:Button") component along with this component on the same [slot](https://wiki.resonite.com/Slot "Slot"), then clicking on the UIX button will prompt for a connection.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Hyperlink&oldid=97951](https://wiki.resonite.com/index.php?title=Component:Hyperlink&oldid=97951)"

Contents