# Component:VolumeUnlitMaterial

> Source: https://wiki.resonite.com/Component:VolumeUnlitMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:VolumeUnlitMaterial&diff=113620) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/ff/VolumeUnlitMaterialComponent.png/510px-VolumeUnlitMaterialComponent.png)](https://wiki.resonite.com/File:VolumeUnlitMaterialComponent.png) **Volume Unlit Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VolumeUnlitMaterial** component is used to display [3D Textures](https://wiki.resonite.com/Texture3D "Texture3D") like Xrays, sunbeams, MRIs, CT scans, or any other 3D texture in a volumetric 3D cube that can optionally be sliced. Can also be used for volumetric lighting, but high texture resolutions can be large and cause considerable render lag.

This is a [raymarched](https://en.wikipedia.org/wiki/Ray_marching) material, which means that a ray is stepped iteratively closer and closer to the volume in order to determine what is shown or not.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `Mode` | **[DisplayMode](https://wiki.resonite.com/Component:VolumeUnlitMaterial#DisplayMode)** | How to display the texture in 3D space. |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |
| `Volume` | **[Texture3D](https://wiki.resonite.com/Type:Texture3D "Type:Texture3D")** | The 3D texture this material should display. |
| `StepSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many cell details there should be. |
| `Gain` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to gain up the color. |
| `Exp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What exponent to raise colors to. |
| `AccumulationCutoff` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | if color goes beyond this brightness, don't render it. |
| `HitThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | tells what value to consider a hit. Any value above this is drawn, and any other value below this is culled. |
| `InputRange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What range duration within 0<->1 do the colors in the 3d image have? Useful for isolating particular ranges for densities in a CT scan. |
| `InputOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | at what point does the range start? |
| `UseAlphaChannel` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the alpha channel in the pixel data of `Volume`. |
| `Slices` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[SlicePlane](https://wiki.resonite.com/Component:VolumeUnlitMaterial#SlicePlane)** | Slice planes that cut the volume along local positions and directions. |
| `Highlights` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[Highlight](https://wiki.resonite.com/Component:VolumeUnlitMaterial#Highlight)** | A list of planes with offsets which define a region of the volume to override the color of. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## DisplayMode

| Name | Value | Description |
| --- | --- | --- |
| `Additive` | 0 | is an "add up over all of the times the ray has intersected the volume" statement. |
| `AdditiveCutoff` | 1 | is an "add up over all of the times the ray has intersected the volume" statement. Respects alpha cutoff. |
| `HitThreshold` | 2 | a binary "has the ray hit the volume or not?". |

Values

## SlicePlane

| Name | Type | Description |
| --- | --- | --- |
| `Normal` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The normal direction of the slice in local space. |
| `Offset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The position of the slice in local space. |

Fields

## Highlight

| Name | Type | Description |
| --- | --- | --- |
| `Normal` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the normal of the plane which defines its orientation in local space. |
| `Offset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far from the center of the volume to offset the plane in the inverse of its normal direction. (For some reason it is the negative of the normal) This is done in local space. |
| `Range` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The "thickness" of the color to add to the volume. This is done on both sides of the plane evenly. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to override with. |

Fields

## Examples

- Khawn2u's RTX world with sunbeams.
- displays for imported 3D textures

- [![This is an originally entirely white volume with a highlight plane which has a normal of <0,1,0>, with no offset, making it centered in the volume. Its range is 0.05 which gives it that thickness. If it was 0.5 this would fill the entire cube, since the volume is size <1,1,1> and this thickness is applied in both directions.](https://wiki.resonite.com/images/thumb/4/4c/Volumetric_Highlights_Example.webp/120px-Volumetric_Highlights_Example.webp.png)](https://wiki.resonite.com/File:Volumetric_Highlights_Example.webp "This is an originally entirely white volume with a highlight plane which has a normal of <0,1,0>, with no offset, making it centered in the volume. Its range is 0.05 which gives it that thickness. If it was 0.5 this would fill the entire cube, since the volume is size <1,1,1> and this thickness is applied in both directions.")

This is an originally entirely white volume with a highlight plane which has a normal of `<0,1,0>`, with no offset, making it centered in the volume. Its range is `0.05` which gives it that thickness. If it was `0.5` this would fill the entire cube, since the volume is size `<1,1,1>` and this thickness is applied in both directions.

- [![In the one on the right the threshold is 0.34, however the red part of the volume has a value of exactly 1/3, meaning that this gets culled, whereas the one on the left the threshold is 0.28 and the red streak passes the hit test and is drawn.](https://wiki.resonite.com/images/thumb/8/8f/Volumetric_HitThreshold_Example.png/120px-Volumetric_HitThreshold_Example.png)](https://wiki.resonite.com/File:Volumetric_HitThreshold_Example.png "In the one on the right the threshold is 0.34, however the red part of the volume has a value of exactly 1/3, meaning that this gets culled, whereas the one on the left the threshold is 0.28 and the red streak passes the hit test and is drawn.")

In the one on the right the threshold is `0.34`, however the red part of the volume has a value of exactly `1/3`, meaning that this gets culled, whereas the one on the left the threshold is `0.28` and the red streak passes the hit test and is drawn.


## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VolumeUnlitMaterial&oldid=113620](https://wiki.resonite.com/index.php?title=Component:VolumeUnlitMaterial&oldid=113620)"

Contents