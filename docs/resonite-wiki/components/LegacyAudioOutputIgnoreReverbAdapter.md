# Component:LegacyAudioOutputIgnoreReverbAdapter

> Source: https://wiki.resonite.com/Component:LegacyAudioOutputIgnoreReverbAdapter

Collapse **Component image**

[File:LegacyAudioOutputIgnoreReverbAdapterComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LegacyAudioOutputIgnoreReverbAdapterComponent.png "File:LegacyAudioOutputIgnoreReverbAdapterComponent.png") **Legacy Audio Output Ignore Reverb Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Legacy Audio Output Ignore Reverb Adapter** component converts driven data from the old audio system to [Awwdio](https://wiki.resonite.com/Awwdio "Awwdio") to preserve legacy behavior.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to drive with the value converted. |
| `Value` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The value to convert. |
| `Spatialize` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | The field that determined if the audio clip was spatialized in the old system. |

Fields
Collapse

## Usage

used only in legacy content.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyAudioOutputIgnoreReverbAdapter&oldid=101118](https://wiki.resonite.com/index.php?title=Component:LegacyAudioOutputIgnoreReverbAdapter&oldid=101118)"

Contents