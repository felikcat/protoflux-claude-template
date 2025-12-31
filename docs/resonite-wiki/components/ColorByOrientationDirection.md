# Component:ColorByOrientationDirection

> Source: https://wiki.resonite.com/Component:ColorByOrientationDirection

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6a/ColorByOrientationDirectionComponent.png/510px-ColorByOrientationDirectionComponent.png)](https://wiki.resonite.com/File:ColorByOrientationDirectionComponent.png) **Color By Orientation Direction** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorByOrientationDirection** component is used to make particles change color depending on their dot product of their orientation to a reference orientation. Dot product essentially means how close in terms of angle is one direction to another. The colors when in-between are lerped.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ReferenceDirection` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction in local space that is being used as a reference. |
| `AlignedColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use if the particle's orientation is exactly the same direction as `ReferenceDirection`. |
| `OrthogonalColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use if the particle's orientation is exactly 90 degrees to `ReferenceDirection`. This 90 degrees falls onto any particle direction that is along the surface of a plane facing the same direction as `ReferenceDirection`. |
| `OppositeColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color if the particle's orientation is exactly opposite of `ReferenceDirection`. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorByOrientationDirection&oldid=96031](https://wiki.resonite.com/index.php?title=Component:ColorByOrientationDirection&oldid=96031)"

Contents