# Component:SphereAligner

> Source: https://wiki.resonite.com/Component:SphereAligner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SphereAligner&diff=106570) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fd/SphereAlignerComponent.png/510px-SphereAlignerComponent.png)](https://wiki.resonite.com/File:SphereAlignerComponent.png) **Sphere Aligner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Sphere aligner is a component that has a list of child slots under `Items` and aligns those items into a spherical shape.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AutoAddChildren` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether slots below this component's slot in the hierarchy are automatically added to `_targets` |
| `AutoAddIgnoreTags` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | Do not add slots to the list of children automatically if it's tag is contained in this list. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the sphere to align items into |
| `DistributionOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Shift the positions of the items along the sphere surface, redistributes. |
| `AlignToNormal` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to rotate the items to align them to the surface of the sphere |
| `RotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | How much to rotate the sphere of aligned items by their individual origins |
| `NormalizedStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What point to start the alignment of items from top to bottom of the sphere. |
| `NormalizedEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What point to end the alignment of items from top to bottom of the sphere. |
| `HorizontalStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What point to start the alignment of items along the equator of the sphere. |
| `HorizontalEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What point to end the alignment of items along the equator of the sphere. |
| `Items` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[SphereAligner.Item](https://wiki.resonite.com/Component:SphereAligner#Item)** | A list of items to align into the sphere shape. |

Fields
Collapse

## Item

| Name | Type | Description |
| --- | --- | --- |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot this is pointing to. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | `Root`'s position field to drive. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | `Root`'s rotation field to drive. |

Fields

## Usage

## Examples

- [SphereAligner tutorial](https://www.youtube.com/watch?v=P07VpBHknts) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SphereAligner&oldid=106570](https://wiki.resonite.com/index.php?title=Component:SphereAligner&oldid=106570)"

Contents