# Component:AnimationTrack

> Source: https://wiki.resonite.com/Component:AnimationTrack

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c8/AnimationTrack%601Component.png/510px-AnimationTrack%601Component.png)](https://wiki.resonite.com/File:AnimationTrack%601Component.png) **Animation Track\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Animation track seems to be a placeholder for future content and is unused. It does not fit into anything in the game internally and it's methods go unused (According to DNSpy 07/26/2024 (mm/dd/yyyy))

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_node` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Designed to be used to specify the object being controlled by the animation. Can be used with the Find Animation Track Index ProtoFlux node. |
| `_component` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Designed to be used to specify the field of the object that is being controlled by the animation. Can be used with the Find Animation Track Index ProtoFlux node. |
| `_property` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The property on an animation asset |
| `Data` | _direct_ **[SyncLinear\`1](https://wiki.resonite.com/index.php?title=Type:SyncLinear%601&action=edit&redlink=1 "Type:SyncLinear`1 (page does not exist)") <T>** | A list of values at specific time intervals to determine what the whole track's value should be at specific times. |

Fields
Collapse

## Behavior

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AnimationTrack&oldid=88749](https://wiki.resonite.com/index.php?title=Component:AnimationTrack&oldid=88749)"

Contents