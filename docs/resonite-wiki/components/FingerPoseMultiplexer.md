# Component:FingerPoseMultiplexer

> Source: https://wiki.resonite.com/Component:FingerPoseMultiplexer

Collapse **Component image**

[File:FingerPoseMultiplexerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FingerPoseMultiplexerComponent.png "File:FingerPoseMultiplexerComponent.png") **Finger Pose Multiplexer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FingerPoseMultiplexer** component can be used to get data from multiple finger pose sources and make that data its own finger pose source data. This component in itself is a [IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent").

For more information on finger pose sources, please see [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | What Component in `Sources` to copy data from for the finger pose data for this component. |
| `InterpolationSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the Multiplexer transitions what data this component is copying for this component's finger pose data. |
| `Sources` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent")** | The list if Finger pose sources to copy data from for the data for this component's Finger pose data. |

Fields
Collapse

## Usage

Add items to the list of `Sources` to transition between and get data from. The data gotten is copied and becomes the data of this component. Can be used in the ways outlined in [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System").

## Examples

[Frooxius devlog video on this component](https://youtu.be/PG4qnZluan4)

## See Also

- [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FingerPoseMultiplexer&oldid=94749](https://wiki.resonite.com/index.php?title=Component:FingerPoseMultiplexer&oldid=94749)"

Contents