# Component:AudioListener

> Source: https://wiki.resonite.com/Component:AudioListener

Collapse **Component image**

[File:AudioListenerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=AudioListenerComponent.png "File:AudioListenerComponent.png") **Audio Listener** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Audio Listener** component can hear audio from the world around it and relay it back. It can also be used as a source for audio data for AudioOutput, working as a virtual microphone (This only works on listeners that aren't bound to specific user - ActiveUser must be null)

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ActiveUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | Position the audio source to this user. |
| `Effects` | _direct_ **[AutoSyncRefList\`1](https://wiki.resonite.com/index.php?title=Type:AutoSyncRefList%601&action=edit&redlink=1 "Type:AutoSyncRefList`1 (page does not exist)") < [AudioDSP\_Effect](https://wiki.resonite.com/Type:AudioDSP_Effect "Type:AudioDSP Effect") >** | The list of affects to apply to the audio this recieves. |

Fields
Collapse

## Usage

Audio Reverb zones and other effects can be dynamically assigned to the list of `Effects` using spatial variables. The default variable for such is "Resonite.Audio.Filters" of type [AudioDSP\_Effect](https://wiki.resonite.com/Type:AudioDSP_Effect "Type:AudioDSP Effect"). Using [SphereConstantReferenceSpatialVariables](https://wiki.resonite.com/Component:SphereConstantReferenceSpatialVariable "Component:SphereConstantReferenceSpatialVariable") of the same type can be used to designate areas with reverbs using the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system.

For audio reverb, the AudioDSP\_Effect the sphere spatial variable component points to needs to be a [Component:AudioFilterBlendWrapper](https://wiki.resonite.com/Component:AudioFilterBlendWrapper "Component:AudioFilterBlendWrapper") with a [Component:AudioZitaReverb](https://wiki.resonite.com/Component:AudioZitaReverb "Component:AudioZitaReverb") in it

The list of effects on this component can be driven using the [ReferenceSpatialVariableDriver](https://wiki.resonite.com/Component:ReferenceSpatialVariableDriver "Component:ReferenceSpatialVariableDriver") and will change depending on what audio effects at it's location it can sample from surrounding [SphereConstantReferenceSpatialVariables](https://wiki.resonite.com/Component:SphereConstantReferenceSpatialVariable "Component:SphereConstantReferenceSpatialVariable")

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioListener&oldid=101089](https://wiki.resonite.com/index.php?title=Component:AudioListener&oldid=101089)"

Contents