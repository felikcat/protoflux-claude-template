# Component:CubemapCreator

> Source: https://wiki.resonite.com/Component:CubemapCreator

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7c/CubemapCreatorComponent.png/510px-CubemapCreatorComponent.png)](https://wiki.resonite.com/File:CubemapCreatorComponent.png) **Cubemap Creator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Cubemap Creator](https://wiki.resonite.com/Cubemap_Creator "Cubemap Creator").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TopBottomRotation` | **[CubemapCreator.Rotation](https://wiki.resonite.com/Component:CubemapCreator#Rotation)** | How to Rotate the top and bottom images to fit. |
| `PosX` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | What to use for the positive X side. |
| `NegX` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | What to use for the negative X side. |
| `PosY` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | What to use for the positive Y side. |
| `NegY` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | What to use for the negative Y side. |
| `PosZ` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | What to use for the top side. |
| `NegZ` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | What to use for the bottom side. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnCreate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Tells the creator to create the cubemap. |

Triggers
Collapse

## Rotation

| Name | Value | Description |
| --- | --- | --- |
| `Default` | 0 | Rotate 0 degrees. |
| `Rotate90CW` | 1 | Rotate 90 degrees clockwise. |
| `Rotate90CCW` | 2 | Rotate 90 degrees counter clockwise. |
| `Rotate180` | 3 | Rotate 180 degrees. |

Values

## Usage

See [Cubemap Creator](https://wiki.resonite.com/Cubemap_Creator "Cubemap Creator").

## Examples

See [Cubemap Creator](https://wiki.resonite.com/Cubemap_Creator "Cubemap Creator").

## See Also

- [Cubemap Creator](https://wiki.resonite.com/Cubemap_Creator "Cubemap Creator")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CubemapCreator&oldid=98397](https://wiki.resonite.com/index.php?title=Component:CubemapCreator&oldid=98397)"

Contents