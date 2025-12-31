# Component:FogBoxVolumeMaterial

> Source: https://wiki.resonite.com/Component:FogBoxVolumeMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:FogBoxVolumeMaterial&diff=113621) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f8/FogBoxVolumeMaterialComponent.png/510px-FogBoxVolumeMaterialComponent.png)](https://wiki.resonite.com/File:FogBoxVolumeMaterialComponent.png) **Fog Box Volume Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Description

The FogBoxVolumeMaterial is a material used to create cube-shaped volumetric fog on a mesh, such as a [Texture3D](https://wiki.resonite.com/Texture3D "Texture3D"). Using this material on non-cube-like meshes may result in visual artifacts and/or denser fog in places where the corners of the cube would be.

Although only cube-shaped meshes are officially supported, users may use the [LookAtUser](https://wiki.resonite.com/Component:LookAtUser "Component:LookAtUser") component targeting the local User along with a spherical mesh to create an illusion of a sphere-shaped fog.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `BaseColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Starting color for the fog volume |
| `AccumulationColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color to use for a Constant fog |
| `AccumulationColorBottom` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color at the end of a Vertical Gradient fog |
| `AccumulationColorTop` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color at the start of a Vertical Gradient fog |
| `FogStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material FogStart](https://wiki.resonite.com/index.php?title=Template:Material_FogStart&action=edit&redlink=1 "Template:Material FogStart (page does not exist)") |
| `FogEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material FogEnd](https://wiki.resonite.com/index.php?title=Template:Material_FogEnd&action=edit&redlink=1 "Template:Material FogEnd (page does not exist)") |
| `FogDensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material FogDensity](https://wiki.resonite.com/index.php?title=Template:Material_FogDensity&action=edit&redlink=1 "Template:Material FogDensity (page does not exist)") |
| `GammaCurve` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The gamma curve of the material colors. |
| `WorldSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | [Template:Material WorldSpace](https://wiki.resonite.com/index.php?title=Template:Material_WorldSpace&action=edit&redlink=1 "Template:Material WorldSpace (page does not exist)") |
| `ColorMode` | **[Color](https://wiki.resonite.com/Component:FogBoxVolumeMaterial#Color)** | [Template:Material ColorMode](https://wiki.resonite.com/index.php?title=Template:Material_ColorMode&action=edit&redlink=1 "Template:Material ColorMode (page does not exist)") |
| `SaturationMode` | **[Saturation](https://wiki.resonite.com/Component:FogBoxVolumeMaterial#Saturation)** | [Template:Material SaturationMode](https://wiki.resonite.com/index.php?title=Template:Material_SaturationMode&action=edit&redlink=1 "Template:Material SaturationMode (page does not exist)") |
| `AccumulationMode` | **[Accumulation](https://wiki.resonite.com/Component:FogBoxVolumeMaterial#Accumulation)** | [Template:Material AccumulationMode](https://wiki.resonite.com/index.php?title=Template:Material_AccumulationMode&action=edit&redlink=1 "Template:Material AccumulationMode (page does not exist)") |
| `AccumulationRate` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | [Template:Material AccumulationRate](https://wiki.resonite.com/index.php?title=Template:Material_AccumulationRate&action=edit&redlink=1 "Template:Material AccumulationRate (page does not exist)") |
| `BlendMode` | **[BlendMode](https://wiki.resonite.com/Type:BlendMode "Type:BlendMode")** | How to blend this material's colors vs what it rendered on top of. |
| `RenderQueue` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | changes at which point a material renders on the render stack |

Fields
Collapse

## Color

| Name | Value | Description |
| --- | --- | --- |
| `Constant` | 0 | A single color fog |
| `VerticalGradient` | 1 | A fog with a gradient pattern |

Values

## Saturation

| Name | Value | Description |
| --- | --- | --- |
| `Unrestricted` | 0 |  |
| `SaturateAlpha` | 1 |  |
| `SaturateColor` | 2 |  |

Values

## Accumulation

| Name | Value | Description |
| --- | --- | --- |
| `Linear` | 0 |  |
| `Exponential` | 1 |  |
| `ExponentialSquared` | 2 |  |

Values

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FogBoxVolumeMaterial&oldid=113621](https://wiki.resonite.com/index.php?title=Component:FogBoxVolumeMaterial&oldid=113621)"

Contents