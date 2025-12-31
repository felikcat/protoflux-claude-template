# Component:MultiTextureFader

> Source: https://wiki.resonite.com/Component:MultiTextureFader

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7b/MultiTextureFader%601Component.png/510px-MultiTextureFader%601Component.png)](https://wiki.resonite.com/File:MultiTextureFader%601Component.png) **Multi Texture Fader\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MultiTextureFader** component can be used with the [Component:PBSLerpMetallic](https://wiki.resonite.com/Component:PBSLerpMetallic "Component:PBSLerpMetallic") or [Component:PBSLerpSpecular](https://wiki.resonite.com/Component:PBSLerpSpecular "Component:PBSLerpSpecular") to lerp multiple textures rather than just one.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FirstTexture` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") <A>** | Usually set to the Texture set 0 of a lerping material. |
| `SecondTexture` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") <A>** | Usually set to the Texture set 1 of a lerping material. The type of texture set like albedo or emission this one is driving should be the same as `FirstTexture`. |
| `Lerp` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The lerp field of the material. Can be left blank if using multiple of this component on the same material. |
| `Position` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The position in the list of `Textures` to fade between. If this is a decimal, the `FirstTexture` and `SecondTexture` will be set to textures in `Textures` that are at the positon of floor and ceiling of this value. |
| `Textures` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **A** | A list of textures to lerp between and set `FirstTexture` and `SecondTexture` to using `Position` to determine the texture from this list. |

Fields
Collapse

## Usage

Can be attached to a slot and given a list of materials. Using a [Component:PBSLerpMetallic](https://wiki.resonite.com/Component:PBSLerpMetallic "Component:PBSLerpMetallic") or [Component:PBSLerpSpecular](https://wiki.resonite.com/Component:PBSLerpSpecular "Component:PBSLerpSpecular") with this component can lerp the list of `Textures` using `Position`. The lerp of the material can be driven via the `Lerp` on this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:PBSLerpMetallic](https://wiki.resonite.com/Component:PBSLerpMetallic "Component:PBSLerpMetallic")
- [Component:PBSLerpSpecular](https://wiki.resonite.com/Component:PBSLerpSpecular "Component:PBSLerpSpecular")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MultiTextureFader&oldid=95131](https://wiki.resonite.com/index.php?title=Component:MultiTextureFader&oldid=95131)"

Contents