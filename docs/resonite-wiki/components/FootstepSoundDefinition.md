# Component:FootstepSoundDefinition

> Source: https://wiki.resonite.com/Component:FootstepSoundDefinition

Collapse **Component image**

[File:FootstepSoundDefinitionComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FootstepSoundDefinitionComponent.png "File:FootstepSoundDefinitionComponent.png") **Footstep Sound Definition** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FootstepSoundDefinition** component can be referenced by other components which can trigger this to play noise during footstep events.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ParentUnder` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to parent played sounds under. |
| `MinDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The minimum distance the audio can be heard from before playing at maximum amount. |
| `MaxDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The max distance before the audio cannot be heard anymore. |
| `RolloffMode` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [AudioRolloffMode](https://wiki.resonite.com/Type:AudioRolloffMode "Type:AudioRolloffMode") >** | How played audio should fall off based on distance. |
| `Clips` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FootstepSoundDefinition.FootstepClip](https://wiki.resonite.com/Component:FootstepSoundDefinition#FootstepClip)** | Different footsteps that can play when this component is triggered |

Fields
Collapse

## FootstepClip

| Name | Type | Description |
| --- | --- | --- |
| `Clip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audioclip to play for this foot step. |
| `Weight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How likely it is for this foot step sound to play. |
| `MinVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum player velocity required for the sound to play. |
| `MaxVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum player velocity allowed for the sound to play. |
| `PlayForWalking` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Should this audio clip be played when the user is walking? |
| `PlayForLanding` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Should this audio clip be played when the user is landing from a jump? |
| `PlayForLeftFoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this sound should be played for the left foot. |
| `PlayForRightFoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this sound should be played for the right foot. |
| `VelocityMinPitch` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum pitch multiplier that can be used with this foot step sound. |
| `VelocityMaxPitch` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum pitch multiplier that can be used with this foot step sound. |
| `PitchMinVelocityReference` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The velocity the player should be moving to map to the minimum pitch for this sound. |
| `PitchMaxVelocityReference` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The velocity the player should be moving to map to the maximum pitch for this sound. |
| `MinPitchVariation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum random amount of pitch to add to the footstep. |
| `MaxPitchVariation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum random amount of pitch to add to the footstep. |
| `VelocityMinVolume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum volume that can be used with this foot step sound. |
| `VelocityMaxVolume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum volume that can be used with this foot step sound. |
| `VolumeMinVelocityReference` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The velocity the player should be moving to map to the minimum volume for this sound. |
| `VolumeMaxVelocityReference` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The velocity the player should be moving to map to the maximum volume for this sound. |
| `MinVolumeVariation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum random amount of volume to add to the footstep. |
| `MaxVolumeVariation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum random amount of volume to add to the footstep. |

Fields

## Usage

Used to play sound when footsteps happen on surfaces or it receives a footstep event.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Footstep components](https://wiki.resonite.com/Category:Components:Locomotion:Footsteps "Category:Components:Locomotion:Footsteps")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FootstepSoundDefinition&oldid=97511](https://wiki.resonite.com/index.php?title=Component:FootstepSoundDefinition&oldid=97511)"

Contents