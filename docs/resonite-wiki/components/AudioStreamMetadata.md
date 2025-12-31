# Component:AudioStreamMetadata

> Source: https://wiki.resonite.com/Component:AudioStreamMetadata

Collapse **Component image**

[File:AudioStreamMetadata\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=AudioStreamMetadata%601Component.png "File:AudioStreamMetadata`1Component.png") **Audio Stream Metadata\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Audio Stream Metadata is a component that reads the running tallies of the different samples being sent and received by an [AudioStream\`1](https://wiki.resonite.com/index.php?title=Type:AudioStream%601&action=edit&redlink=1 "Type:AudioStream`1 (page does not exist)").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Stream` | **[AudioStream\`1](https://wiki.resonite.com/index.php?title=Type:AudioStream%601&action=edit&redlink=1 "Type:AudioStream`1 (page does not exist)") <S>** | The audio source to get data from |
| `UnreadSamples` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of samples yet to be played |
| `TotalMissedSamples` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Samples missed due to lag or other reasons. |
| `LastMissedSamples` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The last time samples were missed instead of being read from the audio source. |
| `BufferLength` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How big the sample buffer is. |
| `AverageReadSamplesPerSecond` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | How many samples per second on a running average are being processed. |
| `AverageWriteSamplesPerSecond` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | The many samples per second on a running average are being written to the buffer per second. |
| `GlobalIndex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Long](https://wiki.resonite.com/Type:Long "Type:Long")** | The audio source's index in the pool of audio players playing sounds. |
| `SamplesAvailableForEncode` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Samples currently ready to be encoded to a format supported by FrooxEngine's audio system. |
| `FrameSize` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The size of audio data coming in, which is in bytes and is influenced by data and channel count. |
| `MaxFrameSize` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The max size of audio data coming in, which is in bytes and is influenced by data and channel count. |
| `EncodedSampleRate` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how fast encoded samples are being processed. |
| `TotalPacketCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many audio packets have been networked by the audio source so far. |
| `TotalLostPackets` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many packets of the network that were not received from the audio source. |
| `LastLostPackets` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The last time packets were lost by the audio source. |
| `PacketLossRatio` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | On average, the percentage of audio packets from the network that are being lost. |
| `AverageCodecSamplesPerSecond` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | The average amount of samples incoming in encoded form. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioStreamMetadata&oldid=93890](https://wiki.resonite.com/index.php?title=Component:AudioStreamMetadata&oldid=93890)"

Contents