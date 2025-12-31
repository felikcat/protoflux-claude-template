# Component:BitmapAssetMetadata

> Source: https://wiki.resonite.com/Component:BitmapAssetMetadata

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/40/BitmapAssetMetadataComponent.png/510px-BitmapAssetMetadataComponent.png)](https://wiki.resonite.com/File:BitmapAssetMetadataComponent.png) **Bitmap Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BitmapAssetMetadata** component is used to get pixel data information on a given image or texture.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Asset` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The image to get data from. |
| `Width` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The width of `Asset`. |
| `Height` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The height of `Asset`. |
| `BaseFormat` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The format of `Asset`. |
| `ColorData` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorChannelData](https://wiki.resonite.com/index.php?title=Type:ColorChannelData&action=edit&redlink=1 "Type:ColorChannelData (page does not exist)")** | The ColorChannelData for `Asset` |
| `AlphaData` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[AlphaChannelData](https://wiki.resonite.com/index.php?title=Type:AlphaChannelData&action=edit&redlink=1 "Type:AlphaChannelData (page does not exist)")** | The AlphaChannelData for `Asset`. |
| `BitsPerPixel` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | How many bits are used per pixel to store color data in `Asset`. |
| `ChannelCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many channels `Asset` has (RGBA for example is 4, but some images may have more or less.) |
| `AverageColor` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | `Asset`'s average color, visible or not. |
| `AverageVisibleColor` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | `Asset`'s average visible color. |
| `AverageHSV` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | `Asset`'s average HSV color, visible ot not. |
| `AverageVisibleHSV` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | `Asset`'s average visible HSV color. |
| `InvalidPixelCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many pixels in `Asset` that have NAN values in their color values. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BitmapAssetMetadata&oldid=93929](https://wiki.resonite.com/index.php?title=Component:BitmapAssetMetadata&oldid=93929)"

Contents