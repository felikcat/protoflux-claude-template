# Component:StreamAudioFacetPreset

> Source: https://wiki.resonite.com/Component:StreamAudioFacetPreset

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/da/StreamAudioFacetPresetComponent.png/510px-StreamAudioFacetPresetComponent.png)](https://wiki.resonite.com/File:StreamAudioFacetPresetComponent.png) **Stream Audio Facet Preset** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **StreamAudioFacetPreset** component loads the Stream Audio facet when it's not `_fullyLoaded`. It does this by loading the facet from the cloud, and using that loaded data to make the preset

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_fullyLoaded` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this facet has been fully loaded and ready to use |

Fields
Collapse

## Usage

used in the main dash. no need to be used by the user unless they are missing the Stream Audio facet.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StreamAudioFacetPreset&oldid=93677](https://wiki.resonite.com/index.php?title=Component:StreamAudioFacetPreset&oldid=93677)"

Contents