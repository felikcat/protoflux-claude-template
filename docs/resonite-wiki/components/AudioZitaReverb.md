# Component:AudioZitaReverb

> Source: https://wiki.resonite.com/Component:AudioZitaReverb

Collapse **Component image**

[File:AudioZitaReverbComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=AudioZitaReverbComponent.png "File:AudioZitaReverbComponent.png") **Audio Zita Reverb** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Audio Zita Reverb** component can be used to create echo effects (called [ZitaParameters](https://wiki.resonite.com/Type:ZitaParameters "Type:ZitaParameters")) onto [audio clips](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip"), or on listeners in an area using the [Awwdio](https://wiki.resonite.com/Awwdio "Awwdio") system. To see how to use it with audio listeners, see [AudioListener](https://wiki.resonite.com/Component:AudioListener "Component:AudioListener").

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you need a way to control reverb using [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux"), use [Construct Zita Parameters](https://wiki.resonite.com/ProtoFlux:Construct_Zita_Parameters "ProtoFlux:Construct Zita Parameters") instead.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `InDelay` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Delay in ms before reverberation begins. |
| `Crossover` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Crossover frequency separating low and middle frequencies (Hz). |
| `RT60Low` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Time (in seconds) to decay 60db in low-frequency band. |
| `RT60Mid` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Time (in seconds) to decay 60db in mid-frequency band. |
| `HighFrequencyDamping` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Frequency (Hz) at which the high-frequency T60 is half the middle-band's T60. |
| `EQ1Frequency` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Center frequency of second-order Regalia Mitra peaking equalizer section 1. |
| `EQ1Level` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Peak level in dB of second-order Regalia-Mitra peaking equalizer section 1 |
| `EQ2Frequency` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Center frequency of second-order Regalia Mitra peaking equalizer section 2. |
| `EQ2Level` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Peak level in dB of second-order Regalia-Mitra peaking equalizer section 2. |
| `Mix` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | 0 is all dry, 1 is all wet. |
| `Level` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Output scale factor (in dB). |

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

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioZitaReverb&oldid=101158](https://wiki.resonite.com/index.php?title=Component:AudioZitaReverb&oldid=101158)"

Contents