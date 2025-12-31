# ProtoFlux:SampleTexture3DUVW

> Source: https://wiki.resonite.com/ProtoFlux:SampleTexture3DUVW

Sample Texture 3D UVW

Texture

\*

UVW

Assets

The **Sample Texture 3D UVW** node allows you to sample the pixel color of a [Texture3D](https://wiki.resonite.com/Texture3D "Texture3D") that has readable enabled based on a 0->1 range on UVW instead of pixels.
Since the [StaticTexture3D](https://wiki.resonite.com/Component:StaticTexture3D "Component:StaticTexture3D") component needs to have readable enabled, most players opt to keep a component on the object that their code is on, and then change it's URL so they can read the image's pixels.

This node also takes a raw [IAsset<Texture3D>](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") instead of an asset provider. To extract the raw texture reference from the provider for use in this node, see the [Get Asset Node](https://wiki.resonite.com/ProtoFlux:Get_Asset "ProtoFlux:Get Asset").

## Inputs

### Texture ( [IAsset<Texture3D>](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1"))

The raw asset of an [IAssetProvider<Texture3D>](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") extracted using a [Get Asset Node](https://wiki.resonite.com/ProtoFlux:Get_Asset "ProtoFlux:Get Asset").

### UVW ( [Float2](https://wiki.resonite.com/Types:Float2 "Types:Float2"))

The UVW position to sample the colorX from.

## Outputs

### \\* ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The ColorX color from the provided Texture ( [IAsset<Texture2D>](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1")) at the provided UVW ( [Float2](https://wiki.resonite.com/Types:Float2 "Types:Float2")).

## Examples

- [Example of a Sample Texture3D UVW being used in a larger example code reading 3D and 2D textures.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_texture_asset_parsing.webp "File:Protoflux texture asset parsing.webp")

Example of a Sample Texture3D UVW being used in a larger example code reading 3D and 2D textures.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SampleTexture3DUVW&oldid=113624](https://wiki.resonite.com/index.php?title=ProtoFlux:SampleTexture3DUVW&oldid=113624)"

Contents