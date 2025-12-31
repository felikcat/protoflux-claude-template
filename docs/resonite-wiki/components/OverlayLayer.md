# Component:OverlayLayer

> Source: https://wiki.resonite.com/Component:OverlayLayer

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:OverlayLayerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=OverlayLayerComponent.png "File:OverlayLayerComponent.png") **Overlay Layer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OverlayLayer** component instructs the renderer to render the hierarchy it is attached to on top of everything else. In [desktop mode](https://wiki.resonite.com/Desktop_Mode "Desktop Mode") the component also causes the hierarchy to render directly in front of the camera, mimicking a 2D user interface.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Behavior

When enabled, OverlayLayer will tell the renderer to render the hierarchy under the slot (including the slot) on top of everything else. Internally, this is done by setting the layer of each GameObject in the hierarchy to `Overlay`.

## Examples

OverlayLayer is used to display the [dash](https://wiki.resonite.com/Dash_Menu "Dash Menu"), [notification panel](https://wiki.resonite.com/index.php?title=Notifications&action=edit&redlink=1 "Notifications (page does not exist)"), and the [cursor](https://wiki.resonite.com/index.php?title=Cursor&action=edit&redlink=1 "Cursor (page does not exist)") on top of everything else in userspace.

## See Also

- [Component:HiddenLayer](https://wiki.resonite.com/Component:HiddenLayer "Component:HiddenLayer")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OverlayLayer&oldid=98837](https://wiki.resonite.com/index.php?title=Component:OverlayLayer&oldid=98837)"

Contents