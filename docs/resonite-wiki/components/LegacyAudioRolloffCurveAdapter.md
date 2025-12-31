# Component:LegacyAudioRolloffCurveAdapter

> Source: https://wiki.resonite.com/Component:LegacyAudioRolloffCurveAdapter

Collapse **Component image**

[File:LegacyAudioRolloffCurveAdapterComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LegacyAudioRolloffCurveAdapterComponent.png "File:LegacyAudioRolloffCurveAdapterComponent.png") **Legacy Audio Rolloff Curve Adapter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Legacy Audio Rolloff Curve Adapter** component is used to convert driven values from the old audio system to [Awwdio](https://wiki.resonite.com/Awwdio "Awwdio").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [AudioRolloffCurve](https://wiki.resonite.com/index.php?title=Type:AudioRolloffCurve&action=edit&redlink=1 "Type:AudioRolloffCurve (page does not exist)") >** | The field to drive with the value converted. |
| `Value` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [AudioRolloffCurve](https://wiki.resonite.com/index.php?title=Type:AudioRolloffCurve&action=edit&redlink=1 "Type:AudioRolloffCurve (page does not exist)") >** | The field being driven by a system using the legacy audio curve settings from before [Awwdio](https://wiki.resonite.com/Awwdio "Awwdio"). |

Fields
Collapse

## Usage

used in legacy content only.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyAudioRolloffCurveAdapter&oldid=101119](https://wiki.resonite.com/index.php?title=Component:LegacyAudioRolloffCurveAdapter&oldid=101119)"

Contents