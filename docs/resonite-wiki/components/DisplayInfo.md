# Component:DisplayInfo

> Source: https://wiki.resonite.com/Component:DisplayInfo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a3/DisplayInfoComponent.png/510px-DisplayInfoComponent.png)](https://wiki.resonite.com/File:DisplayInfoComponent.png) **Display Info** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DisplayInfo** component is used to get information about the local user's display.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DisplayIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The display index to get info on. |
| `Resolution` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The resolution of display `DisplayIndex` |
| `Offset` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The offset of pixels of display `DisplayIndex` |
| `DPI` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The Dots Per Inch of display `DisplayIndex` |
| `RefreshRate` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | The refresh rate in Hertz of `DisplayIndex` |
| `Orientation` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[RectOrientation](https://wiki.resonite.com/index.php?title=Type:RectOrientation&action=edit&redlink=1 "Type:RectOrientation (page does not exist)")** | The orientation of `DisplayIndex`. |
| `IsPrimary` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether display `DisplayIndex` is the main monitor in the OS. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DisplayInfo&oldid=93759](https://wiki.resonite.com/index.php?title=Component:DisplayInfo&oldid=93759)"

Contents