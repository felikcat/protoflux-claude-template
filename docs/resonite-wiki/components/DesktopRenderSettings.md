# Component:DesktopRenderSettings

> Source: https://wiki.resonite.com/Component:DesktopRenderSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/aa/DesktopRenderSettingsComponent.png/510px-DesktopRenderSettingsComponent.png)](https://wiki.resonite.com/File:DesktopRenderSettingsComponent.png) **Desktop Render Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DesktopRenderSettings** component is used to set [Settings](https://wiki.resonite.com/Settings "Settings") used in Desktop mode.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FieldOfView` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The fov of the desktop client. |
| `SprintFieldOfViewZoom` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to multiply the FOV when sprinting |
| `VSync` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use VSync |
| `LimitFramerateWhenUnfocused` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to limit framerate when the game is unfocused. |
| `MaximumBackgroundFramerate` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How much to limit the framerate when unfocused and `LimitFramerateWhenUnfocused` is true. |
| `FramePacingOptionsEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to pace frames due to options like `MaximumBackgroundFramerate` is being used. |
| `BackgroundFramerateEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to render new frames when in the background. |

Fields
Collapse

## Usage

## Examples

## See Also

- [Desktop Render Settings](https://wiki.resonite.com/Settings#Desktop_Render_Settings "Settings")
- [Dash](https://wiki.resonite.com/Dash "Dash")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DesktopRenderSettings&oldid=93789](https://wiki.resonite.com/index.php?title=Component:DesktopRenderSettings&oldid=93789)"

Contents