# Component:TextureQualitySettings

> Source: https://wiki.resonite.com/Component:TextureQualitySettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4f/TextureQualitySettingsComponent.png/510px-TextureQualitySettingsComponent.png)](https://wiki.resonite.com/File:TextureQualitySettingsComponent.png) **Texture Quality Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextureQualitySettings** component is part of the [Settings](https://wiki.resonite.com/Settings "Settings") menu and should be interacted with via such menu instead of through this component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TextureSizeRatio` | **[TextureSizeRatio](https://wiki.resonite.com/Type:TextureSizeRatio "Type:TextureSizeRatio")** | The ratio at which textures should be loaded locally versus their original size on the cloud. |
| `TextureSizeLimit` | **[TextureSizeLimit](https://wiki.resonite.com/Type:TextureSizeLimit "Type:TextureSizeLimit")** | The maximum Texture Size that textures should be loaded at. |
| `MinimumTextureSize` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The minimum size textures loaded can be locally. |
| `DefaultFilterMode` | **[TextureFilterMode](https://wiki.resonite.com/Type:TextureFilterMode "Type:TextureFilterMode")** | The default Texture mode that textures will be if they don't manually specify their Texture mode. |
| `AnisotropicLevel` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The Anisotropic levels textures should have. |
| `UseAnisotropicLevel` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the Anisotropic levels should be used. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `ReloadAllTextures:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Forces a reload of all loaded textures to use curre t Settings (LAGGY) |

Triggers
Collapse

## Usage

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Examples

See [Settings](https://wiki.resonite.com/Settings "Settings").

## See Also

- [Settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextureQualitySettings&oldid=100742](https://wiki.resonite.com/index.php?title=Component:TextureQualitySettings&oldid=100742)"

Contents