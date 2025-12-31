# Component:ButtonPlaybackSeeker

> Source: https://wiki.resonite.com/Component:ButtonPlaybackSeeker

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ButtonPlaybackSeeker&diff=90374) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ed/ButtonPlaybackSeekerComponent.png/510px-ButtonPlaybackSeekerComponent.png)](https://wiki.resonite.com/File:ButtonPlaybackSeekerComponent.png) **Button Playback Seeker** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonPlaybackSeeker** component takes in an [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable"). When a user uses thier laser on an [IButton](https://wiki.resonite.com/Type:IButton "Type:IButton") that also has connections to a slider or set of values that allow it to slide, this component will determine how to interpret that interaction to the seek bar of the IPlayable media.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Playback` | **[IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")** | The media to seek through. |
| `Vertical` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, the button will interpret the seek bar as vertical instead of horizontal. |
| `Continuous` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, allows the user to hold down the laser on the seek bar button and have it constantly change as the laser moves around. |

Fields
Collapse

## Usage

This just gives extra functionality or options to control your media.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonPlaybackSeeker&oldid=90374](https://wiki.resonite.com/index.php?title=Component:ButtonPlaybackSeeker&oldid=90374)"

Contents