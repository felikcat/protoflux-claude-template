# Component:TextureSheetAnimator

> Source: https://wiki.resonite.com/Component:TextureSheetAnimator

Collapse **Component image**

[File:TextureSheetAnimatorComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=TextureSheetAnimatorComponent.png "File:TextureSheetAnimatorComponent.png") **Texture Sheet Animator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextureSheetAnimator** component makes particles animate their texture over lifetime or duration.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TileGridSize` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The amount of cells and rows that the texture atlas sheet has. |
| `AnimationCycleCount` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many times to cycle the animation during the specified time frame. |
| `AnimationType` | **[TextureSheetAnimationType](https://wiki.resonite.com/index.php?title=Type:TextureSheetAnimationType&action=edit&redlink=1 "Type:TextureSheetAnimationType (page does not exist)")** | The animation type to use for the texture sheet animation. |
| `RowIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The row index to start on. |
| `UseRandomRow` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to start the texture sheet animation in a random row. |
| `StartWithRandomOffset` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Start the texture sheet animation in a random column. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

Can be used to make burning fire, or twinkling stars on particles.

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextureSheetAnimator&oldid=96057](https://wiki.resonite.com/index.php?title=Component:TextureSheetAnimator&oldid=96057)"

Contents