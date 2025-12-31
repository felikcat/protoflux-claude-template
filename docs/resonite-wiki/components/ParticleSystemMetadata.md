# Component:ParticleSystemMetadata

> Source: https://wiki.resonite.com/Component:ParticleSystemMetadata

Collapse **Component image**

[File:ParticleSystemMetadataComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ParticleSystemMetadataComponent.png "File:ParticleSystemMetadataComponent.png") **Particle System Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Particle System Metadata** component gives running status numbers for a given [ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `System` | **[ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")** | the particle system to get data from. |
| `ParticleCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The current particle count of `System`. |
| `ParticlesFPS` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current simulation FPS of `System`. |
| `LastSimulationTime` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The seconds needed to do the last simulation of `System`. |
| `LastSubmissionTime` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the seconds needed to do the last submission of data to the renderer for `System`. |
| `RenderDataReallocationCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of reallocation needed for the render data for `System`. |
| `TrailCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of current trails in `System`. |
| `TrailCapacity` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The trail capacity for trail point groups of the current trail buffer pool of `System`. |
| `TrailPointCapacity` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The trail capacity for trail points of the current trail buffer pool of `System`. |
| `TrailsDataReallocationCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of reallocation needed for the render data for trails of `System`. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Seen at the bottom of [ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem") components in the inspector.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ParticleSystemMetadata&oldid=98790](https://wiki.resonite.com/index.php?title=Component:ParticleSystemMetadata&oldid=98790)"

Contents