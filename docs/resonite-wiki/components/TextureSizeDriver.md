# Component:TextureSizeDriver

> Source: https://wiki.resonite.com/Component:TextureSizeDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TextureSizeDriver&diff=97782) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6e/TextureSizeDriverComponent.png/510px-TextureSizeDriverComponent.png)](https://wiki.resonite.com/File:TextureSizeDriverComponent.png) **Texture Size Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextureSizeDriver** component drives a field with the size of a texture in pixels.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to get a size from. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The value field to drive with the final result value. |
| `DriveMode` | **[TextureSizeDriver.Mode](https://wiki.resonite.com/Component:TextureSizeDriver#Mode)** | The way of restricting `Texture` size values as second step. |
| `Premultiply` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The value to multiply the `Texture` size by as first step. |
| `Ratio` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The value to multiply the `Texture` size by as the third step. |
| `MaxSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The value to restrict the output value to be less than this as the final step. |

Fields
Collapse

## Mode

| Name | Value | Description |
| --- | --- | --- |
| `Absolute` | 0 | Use the `Texture` size without modifying the value. |
| `UnitHeight` | 1 | Take the `Texture` size and divide it by the height of the texture. |
| `UnitWidth` | 2 | Take the `Texture` size and divide it by the width of the texture. |
| `Normalized` | 3 | treat the `Texture` size as a vector and normalize it. |

Values

## Usage

Attach to a slot and provide a `Texture` and a `Target` to get started.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextureSizeDriver&oldid=97782](https://wiki.resonite.com/index.php?title=Component:TextureSizeDriver&oldid=97782)"

Contents