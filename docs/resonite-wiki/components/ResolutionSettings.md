# Component:ResolutionSettings

> Source: https://wiki.resonite.com/Component:ResolutionSettings

**Component image**

[![](https://wiki.resonite.com/images/thumb/c/c7/ResolutionSettingsComponent.png/510px-ResolutionSettingsComponent.png)](https://wiki.resonite.com/File:ResolutionSettingsComponent.png) **Resolution Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ResolutionSettings** component is a [Settings](https://wiki.resonite.com/Settings "Settings") component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Fullscreen` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the game should change to fullscreen mode. |
| `WindowResolution` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The resolution in pixels the main window should render at while in windowed mode. |
| `FullscreenResolution` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The resolution in pixels the main window should render at while in full screen. |
| `CommitedWindowResolution` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The resolution in pixels the main window is currently at while in windowed mode. |
| `CommitedFullscreenResolution` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The resolution in pixels the main window is currently at while in full screen. |
| `NeedsToApplyResolution` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the resolution settings need to be applied. |

Fields

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `ApplyResolution:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Applies the currently chosen resolution. |

Triggers

## Usage

See [Resolution Settings](https://wiki.resonite.com/Settings#Resolution "Settings").

## Examples

See [Resolution Settings](https://wiki.resonite.com/Settings#Resolution "Settings").

## See Also

- [Resolution Settings](https://wiki.resonite.com/Settings#Resolution "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ResolutionSettings&oldid=99159](https://wiki.resonite.com/index.php?title=Component:ResolutionSettings&oldid=99159)"

Contents