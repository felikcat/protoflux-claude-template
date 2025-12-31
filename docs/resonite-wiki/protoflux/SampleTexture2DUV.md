# ProtoFlux:SampleTexture2DUV

> Source: https://wiki.resonite.com/ProtoFlux:SampleTexture2DUV

Sample Texture 2D UV

Texture

\*

UV

WrapMode

Assets

Sample texture 2D UV is a node that allows you to sample the pixel color of an [2 dimensional Texture](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") that has readable enabled based on a 0->1 range on UV instead of pixels.
Since the [StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D") component needs to have readable enabled, most players opt to keep a component on the object that their code is on, and then change it's URL so they can read the image's pixels.

This node also takes a raw [IAsset<Texture2D>](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") instead of an asset provider. To extract the raw texture reference from the provider for use in this node, see the [Get Asset Node](https://wiki.resonite.com/ProtoFlux:Get_Asset "ProtoFlux:Get Asset").

## Inputs

### Texture ( [IAsset<Texture2D>](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1"))

The raw asset of an [IAssetProvider<Texture2D>](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") extracted using a [Get Asset Node](https://wiki.resonite.com/ProtoFlux:Get_Asset "ProtoFlux:Get Asset").

### UV ( [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The UV position to sample the colorX from.

### WrapMode ( [WrapMode](https://wiki.resonite.com/Type:WrapMode "Type:WrapMode"))

Which mode should be used when sampling past the UV 0-1 space.

## Outputs

### \\* ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The ColorX color from the provided Texture ( [IAsset<Texture2D>](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1")) at the provided UV Position ( [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")).

## Examples

- [![Example of GetTexture2DPixel And SampleTexture2DUV sampling color from a generated UV texture](https://wiki.resonite.com/images/thumb/6/66/GetTexture2DPixelAndSampleTexture2DUV.png/480px-GetTexture2DPixelAndSampleTexture2DUV.png)](https://wiki.resonite.com/File:GetTexture2DPixelAndSampleTexture2DUV.png "Example of GetTexture2DPixel And SampleTexture2DUV sampling color from a generated UV texture")

Example of GetTexture2DPixel And SampleTexture2DUV sampling color from a generated UV texture


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SampleTexture2DUV&oldid=114751](https://wiki.resonite.com/index.php?title=ProtoFlux:SampleTexture2DUV&oldid=114751)"

Contents