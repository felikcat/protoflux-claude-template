# Component:AlphaOverLifetimeLinearGradient

> Source: https://wiki.resonite.com/Component:AlphaOverLifetimeLinearGradient

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/17/AlphaOverLifetimeLinearGradientComponent.png/510px-AlphaOverLifetimeLinearGradientComponent.png)](https://wiki.resonite.com/File:AlphaOverLifetimeLinearGradientComponent.png) **Alpha Over Lifetime Linear Gradient** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AlphaOverLifetimeLinearGradient** component implements the older alpha over lifetime system that came from Unity. It allows for particles to change alpha depending on how long they have existed for.

A more modern alternative to this with actual editablilty is the [ColorOverLifetimeTexture](https://wiki.resonite.com/Component:ColorOverLifetimeTexture "Component:ColorOverLifetimeTexture") component.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AlphaOverLifetime` | _direct_ **[SyncLinear\`1](https://wiki.resonite.com/index.php?title=Type:SyncLinear%601&action=edit&redlink=1 "Type:SyncLinear`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The Linear Gradient of alpha values to use over lifetime. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetupAlphaFadeInFadeOut:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | transition template going from 0% - 10%, 90% - 100% |
| `SetupAlphaFadeOut:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | transition template going from 90% - 100% |
| `SetupAlphaFadeIn:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | transition template going from 0% - 10% |
| `ClearFadeEffects:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Clear transition template. |

Triggers
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

## See Also

- [Component:ColorOverLifetimeStartEnd](https://wiki.resonite.com/Component:ColorOverLifetimeStartEnd "Component:ColorOverLifetimeStartEnd")
- [Component:ColorHSV OverLifetimeStartEnd](https://wiki.resonite.com/Component:ColorHSV_OverLifetimeStartEnd "Component:ColorHSV OverLifetimeStartEnd")
- [Component:ColorOverLifetimeTexture](https://wiki.resonite.com/Component:ColorOverLifetimeTexture "Component:ColorOverLifetimeTexture")
- Component:AlphaOverLifetimeLinearGradient
- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AlphaOverLifetimeLinearGradient&oldid=98318](https://wiki.resonite.com/index.php?title=Component:AlphaOverLifetimeLinearGradient&oldid=98318)"

Contents