# Component:ColorBySpeedTexture

> Source: https://wiki.resonite.com/Component:ColorBySpeedTexture

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8d/ColorBySpeedTextureComponent.png/510px-ColorBySpeedTextureComponent.png)](https://wiki.resonite.com/File:ColorBySpeedTextureComponent.png) **Color By Speed Texture** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Color By Speed Texture** component samples from the x axis of the UV depending on the min and max speeds being a 0-1 range and values beyond the range being extrapolated.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MinSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed the particle has to be be traveling at or under to be considered minimum speed. |
| `MaxSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed the particle has to be be traveling at or above to be considered maximum speed. |
| `U_WrapMode` | **[WrapMode](https://wiki.resonite.com/Type:WrapMode "Type:WrapMode")** | How to wrap around the X axis. |
| `Texture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to sample color from. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorBySpeedTexture&oldid=98342](https://wiki.resonite.com/index.php?title=Component:ColorBySpeedTexture&oldid=98342)"

Contents