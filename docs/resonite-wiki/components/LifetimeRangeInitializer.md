# Component:LifetimeRangeInitializer

> Source: https://wiki.resonite.com/Component:LifetimeRangeInitializer

**Component image**
[File:LifetimeRangeInitializerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LifetimeRangeInitializerComponent.png "File:LifetimeRangeInitializerComponent.png") **Lifetime Range Initializer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")
The **LifetimeRangeInitializer** component makes particles in a particle system start with a random lifetime/duration within a range.
This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").
## Fields
Fields  Name  | Type  | Description
---|---|---
`persistent` |  | Determines whether or not this item will be saved to the server.
`UpdateOrder` | Controls the order in which this component is updated.
`Enabled` |  | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't.
`MinValue` |  | The minimum lifetime a particle can start with.
`MaxValue` |  | The maximum lifetime a particle can start with.
## Usage
Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.
## Examples
_This article or section is a stub. You can help the Resonite wiki by expanding it._
## See Also
  * [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
