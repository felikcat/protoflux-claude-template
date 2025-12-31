# Component:ColorByVelocityDirection

> Source: https://wiki.resonite.com/Component:ColorByVelocityDirection

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bb/ColorByVelocityDirectionComponent.png/510px-ColorByVelocityDirectionComponent.png)](https://wiki.resonite.com/File:ColorByVelocityDirectionComponent.png) **Color By Velocity Direction** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Color By Velocity Direction** component changes the color of a particle depending on the dot product of it's velocity vs a specified axis.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ReferenceDirection` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction to make a dot product with the particle's velocity. |
| `AlignedColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the particle should be when it has velocity that gives dot product of 1 with `ReferenceDirection`. |
| `OrthogonalColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the particle should be when it has velocity that gives dot product of 0 with `ReferenceDirection`. |
| `OppositeColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the particle should be when it has velocity that gives dot product of -1 with `ReferenceDirection`. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorByVelocityDirection&oldid=98343](https://wiki.resonite.com/index.php?title=Component:ColorByVelocityDirection&oldid=98343)"

Contents