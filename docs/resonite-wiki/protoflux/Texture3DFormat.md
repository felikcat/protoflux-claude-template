# ProtoFlux:Texture3DFormat

> Source: https://wiki.resonite.com/ProtoFlux:Texture3DFormat

Texture 3D Format

Texture

Size

Format

MipMapCount

Assets

The **Texture 3D Format** node returns some of the MetaData associated with a [StaticTexture3D Component](https://wiki.resonite.com/Component:StaticTexture3D "Component:StaticTexture3D") in a [Texture3D](https://wiki.resonite.com/Texture3D "Texture3D").

## Inputs

### Texture ( [IAsset\`1](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") < [Texture3D](https://wiki.resonite.com/Texture3D "Texture3D") >)

The texture to read the metadata for.

## Outputs

### Size ( [int3](https://wiki.resonite.com/Type:Int3 "Type:Int3"))

The size of the texture in pixels.

### Format ( [TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat"))

The [TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat") the texture is in.

### MipMapCount ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

How many mipmap levels this texture has.

## Examples

- [Example of a Texture3D Format being used in a larger example code reading 3D and 2D textures.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_texture_asset_parsing.webp "File:Protoflux texture asset parsing.webp")

Example of a Texture3D Format being used in a larger example code reading 3D and 2D textures.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Texture3DFormat&oldid=113612](https://wiki.resonite.com/index.php?title=ProtoFlux:Texture3DFormat&oldid=113612)"

Contents