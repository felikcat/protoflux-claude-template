# Component:GradientSkyMaterial

> Source: https://wiki.resonite.com/Component:GradientSkyMaterial

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:GradientSkyMaterial&diff=105829) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f8/GradientSkyMaterialComponent.png/510px-GradientSkyMaterialComponent.png)](https://wiki.resonite.com/File:GradientSkyMaterialComponent.png) **Gradient Sky Material** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GradientSkyMaterial** component is used in [Component:Skybox](https://wiki.resonite.com/Component:Skybox "Component:Skybox") to make a gradient type sky for use in worlds.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `_shader` | **[Shader](https://wiki.resonite.com/Type:Shader "Type:Shader")** | Internal. |
| `BaseColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Starting color for the fog volume |
| `_gradients` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[Gradient](https://wiki.resonite.com/Component:GradientSkyMaterial#Gradient)** | Applies a list of [Gradients](https://wiki.resonite.com/Component:GradientSkyMaterial#Gradient) to the sky. |

Fields
Collapse

## Usage

Attach to a slot and insert into a [Component:Skybox](https://wiki.resonite.com/Component:Skybox "Component:Skybox") component and use the SetCurrentSky() Sync Method to use this component. Don't forget to add some `_gradients` to the list.

## Gradient

**Gradient** is a nested type used in the `_gradients` list.

| Name | Type | Description |
| --- | --- | --- |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction this gradient should point in. |
| `FromColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to start at for this gradient. |
| `ToColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to end at for this gradient. |
| `Spread` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to extend the gradient from it's `From` and `To` limits beyond the transitioning section. |
| `From` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where this gradient should start from in a range from 0<->1 |
| `To` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Where this gradient should end at in a range from 0<->1 |
| `Exp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The sharpness of the transition of the gradient |

Fields

## Examples

- [Basic World Creation Pt. 1 Simple World](https://www.youtube.com/watch?v=8hWVylVttmg) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## Related Components

- [Component:Skybox](https://wiki.resonite.com/Component:Skybox "Component:Skybox")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GradientSkyMaterial&oldid=105829](https://wiki.resonite.com/index.php?title=Component:GradientSkyMaterial&oldid=105829)"

Contents