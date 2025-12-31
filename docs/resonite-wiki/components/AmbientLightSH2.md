# Component:AmbientLightSH2

> Source: https://wiki.resonite.com/Component:AmbientLightSH2

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a4/AmbientLightSH2Component.png/510px-AmbientLightSH2Component.png)](https://wiki.resonite.com/File:AmbientLightSH2Component.png) **Ambient Light SH2** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Ambient Light SH2** component creates ambient lighting data that creates global colored light using sampling from a Level 2 Spherical Harmonic type ColorX.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AmbientLight` | **[SphericalHarmonicsL2\`1](https://wiki.resonite.com/Type:SphericalHarmonicsL2%601 "Type:SphericalHarmonicsL2`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The spherical harmonic to sample for ambient lighting. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetActive:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Make this ambient lighting component the current world ambient light. |

Triggers
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AmbientLightSH2&oldid=98925](https://wiki.resonite.com/index.php?title=Component:AmbientLightSH2&oldid=98925)"

Contents