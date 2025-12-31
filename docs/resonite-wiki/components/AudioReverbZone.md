# Component:AudioReverbZone

> Source: https://wiki.resonite.com/Component:AudioReverbZone

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AudioReverbZone&diff=101093) which are not marked for translation.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c7/AudioReverbZoneComponent.png/510px-AudioReverbZoneComponent.png)](https://wiki.resonite.com/File:AudioReverbZoneComponent.png) **Audio Reverb Zone** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Audio reverb zones are used to make audio have an echo effect or a tin can sounding effect. Currently, audio reverb zones only work on un-spacialized audio, like global voice mode.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MinDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the minimum distance that this will affect audio sources from its slot position in global space. Below this distance audio sources will be 100% affected by this reverb zone. |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum distance that this will affect audio sources from its slot position in global space. From minimum distance to this distance it falls off in power until it hits 0 at this distance. |
| `Room` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The size of the room |
| `RoomHF` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Relative room effect level at high frequencies. |
| `RoomLF` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Relative room effect level at low frequencies. |
| `DecayTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how long it takes for sound to fully die out in the room |
| `DecayHFRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | High-frequency to mid-frequency decay time ratio. |
| `Reflections` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | max reflections that can happen in the room. |
| `ReflectionsDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the delay before reflections also known as echos come back and repeat themselves. |
| `Reverb` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many times the sound can reverb |
| `ReverbDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the time it takes for the reverb to return |
| `HFReference` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Reference high frequency (hz). |
| `LFReference` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Reference low frequency (hz). |
| `Diffusion` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much the sound will propagate across the room |
| `Density` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how dense the air is in the room. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SetPreset:ButtonEventHandler`1<Action>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Action](https://wiki.resonite.com/Type:Action "Type:Action") >** | ✓ | Runs the provided action to apply a preset. |
| `PresetOff:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to not have an effect at all |
| `PresetGeneric:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetPaddedCell:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetRoom:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetBathroom:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetLivingroom:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetStoneroom:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetAuditorium:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetConcerthall:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetCave:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetArena:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetHangar:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetCarpetedHallway:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetHallway:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetStoneCorridor:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetAlley:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetForest:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetCity:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetMountains:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetQuarry:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetPlain:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetParkingLot:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetSewerPipe:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetUnderwater:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetDrugged:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetDizzy:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |
| `PresetPsychotic:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Sets the values to a preset that replicates this button's name |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Can be used to make global audio echo or sound like it's inside of a tin can.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioReverbZone&oldid=101093](https://wiki.resonite.com/index.php?title=Component:AudioReverbZone&oldid=101093)"

Contents