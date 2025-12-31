# Component:UniverseStatus

> Source: https://wiki.resonite.com/Component:UniverseStatus

Collapse **Component image**

[File:UniverseStatusComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=UniverseStatusComponent.png "File:UniverseStatusComponent.png") **Universe Status** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UniverseStatus** component provides information on the current [universe](https://wiki.resonite.com/Universes "Universes").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UniverseId` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The ID of the universe current Universe. |
| `UniverseName` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The universe's name. |
| `PrimaryGroupId` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The ID of the primary group of the universe. |
| `InUniverse` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether we are in a universe or not. |

Fields
Collapse

## Usage

Attach to a slot and it will start giving data on the current universe.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Universes](https://wiki.resonite.com/Universes "Universes")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UniverseStatus&oldid=95821](https://wiki.resonite.com/index.php?title=Component:UniverseStatus&oldid=95821)"

Contents