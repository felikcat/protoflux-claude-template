# Component:PlaybackStateDriver

> Source: https://wiki.resonite.com/Component:PlaybackStateDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PlaybackStateDriver&diff=92454) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bb/PlaybackStateDriverComponent.png/510px-PlaybackStateDriverComponent.png)](https://wiki.resonite.com/File:PlaybackStateDriverComponent.png) **Playback State Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PlaybackStateDriver** is a component that drives a set of booleans to whether or not certain states are currently active or not for a particular [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")** | Playback source - VideoTextureProvider or Playback |
| `IsPlaying` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Will drive IField<bool> to true if playing, false if not playing |
| `IsNotPlaying` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Will drive IField<bool> to true is not playing, false if playing |
| `IsPaused` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Will drive IField<bool> to true if playable is paused |
| `IsStopped` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Will drive IField<bool> to true if playable is stopped |

Fields
Collapse

## Usage

Attach to a slot and provide `Source` any [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") provided to the other fields will be driven to the status of that field's status check.

## Examples

[![Example of PlaybackStateDriver](https://wiki.resonite.com/images/thumb/0/0b/PlaybackStateDriverExample1.png/512px-PlaybackStateDriverExample1.png)](https://wiki.resonite.com/File:PlaybackStateDriverExample1.png "Example of PlaybackStateDriver")
The Source (being driven by a VideoTextureProvider) is driving the ValueField<bool> Value to true, since the video is playing.

## See Also

- [Component:IsPlayingDriver](https://wiki.resonite.com/Component:IsPlayingDriver "Component:IsPlayingDriver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PlaybackStateDriver&oldid=92454](https://wiki.resonite.com/index.php?title=Component:PlaybackStateDriver&oldid=92454)"

Contents