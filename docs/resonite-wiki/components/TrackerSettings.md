# Component:TrackerSettings

> Source: https://wiki.resonite.com/Component:TrackerSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/35/TrackerSettingsComponent.png/510px-TrackerSettingsComponent.png)](https://wiki.resonite.com/File:TrackerSettingsComponent.png) **Tracker Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Settings/Tracker Settings](https://wiki.resonite.com/Settings#Tracker_Settings "Settings")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UseTrackers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If all body trackers should be enabled. |
| `Trackers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[TrackerSettings.Tracker](https://wiki.resonite.com/Component:TrackerSettings#Tracker)** | View all names, assignments, ids, and statuses for previously used trackers. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `GetTrackerForSubsetting:SubsettingGetter` | **[SubsettingGetter](https://wiki.resonite.com/Type:SubsettingGetter "Type:SubsettingGetter")** | X | Gets one of the `Trackers` by key. |

Triggers
Collapse

## Tracker

| Name | Type | Description |
| --- | --- | --- |
| `UseTracker` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the tracker right now. |
| `FreezeTracking` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Freeze the tracking into it's last reported position |
| `IsConnected` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this tracker is connected to the game or not, usually means it's not connected to steamvr if this is false. |
| `CustomName` | **[string](https://wiki.resonite.com/Type:String "Type:String")** | A custom name set by the user to identify the tracker. |
| `MappedBodyNode` | **[BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")** | The node which this tracker should be used to track. |
| `MappedPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset position for mapping to the body |
| `MappedRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The offset rotation for mapping to the body |
| `UseInVR` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use this tracker while the user is in VR mode. |
| `UseInDesktop` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use this tracker while the user is in desktop mode. |
| `TrackerID` | **[string](https://wiki.resonite.com/Type:String "Type:String")** | The ID of the tracker, usually designated by the manufacturer of the tracker. |
| `TrackerBattery` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much battery the tracker has left. |
| `TrackerIsCharging` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the tracker is currently charging. |

Fields

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TrackerSettings&oldid=106595](https://wiki.resonite.com/index.php?title=Component:TrackerSettings&oldid=106595)"

Contents