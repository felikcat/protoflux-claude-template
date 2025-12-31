# Component:DirectVisemeDriver

> Source: https://wiki.resonite.com/Component:DirectVisemeDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3e/DirectVisemeDriverComponent.png/510px-DirectVisemeDriverComponent.png)](https://wiki.resonite.com/File:DirectVisemeDriverComponent.png) **Direct Viseme Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DirectVisemeDriver** component takes a viseme analyser source and a few modifying sources in order to drive a list of [Visemes](https://wiki.resonite.com/Visemes "Visemes").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[VisemeAnalyzer](https://wiki.resonite.com/Component:VisemeAnalyzer "Component:VisemeAnalyzer")** | The viseme analyser used as a source of data. |
| `MouthTrackingSource` | **[IMouthTrackingSourceComponent](https://wiki.resonite.com/Type:IMouthTrackingSourceComponent "Type:IMouthTrackingSourceComponent")** | A source of mouth tracking that influences final results. Use a [Component:AvatarMouthDataSourceAssigner](https://wiki.resonite.com/Component:AvatarMouthDataSourceAssigner "Component:AvatarMouthDataSourceAssigner") To assign to this automatically. |
| `StrengthMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to multiply the values from `Source` before sending them to the drives on this component. |
| `VoiceMouthSupressWeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much visemes should be affected by `MouthTrackingSource` if the user is not talking. Lower values mean the affect from `MouthTrackingSource` is greater. |
| `LaughThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much probability for laughter is needed before it sends it to `Laugh` |
| `LaughBeginSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast `Laugh` transitions to 100%. |
| `LaughEndSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast `Laugh` transitions to 0%. |
| `Silence` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How quiet the source data is overall. |
| `PP` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `PP` from `Source` after applying filters from this component. |
| `FF` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `FF` from `Source` after applying filters from this component. |
| `TH` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `TH` from `Source` after applying filters from this component. |
| `DD` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `DD` from `Source` after applying filters from this component. |
| `kk` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `kk` from `Source` after applying filters from this component. |
| `CH` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `CH` from `Source` after applying filters from this component. |
| `SS` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `SS` from `Source` after applying filters from this component. |
| `nn` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `nn` from `Source` after applying filters from this component. |
| `RR` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `RR` from `Source` after applying filters from this component. |
| `aa` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `aa` from `Source` after applying filters from this component. |
| `E` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `E` from `Source` after applying filters from this component. |
| `ih` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `ih` from `Source` after applying filters from this component. |
| `oh` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `oh` from `Source` after applying filters from this component. |
| `ou` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `ou` from `Source` after applying filters from this component. |
| `Laugh` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with `Laugh` from `Source` after applying filters from this component. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `AutoAssignTargets:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Assigns the blendshapes from the first [Component:SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer") based on the matching rules from [Visemes](https://wiki.resonite.com/Visemes "Visemes") to the drive fields of this component. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

- [Component:VisemeAnalyzer](https://wiki.resonite.com/Component:VisemeAnalyzer "Component:VisemeAnalyzer")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DirectVisemeDriver&oldid=97923](https://wiki.resonite.com/index.php?title=Component:DirectVisemeDriver&oldid=97923)"

Contents