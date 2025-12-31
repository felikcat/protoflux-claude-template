# Component:NameplateVisibilityFacetPreset

> Source: https://wiki.resonite.com/Component:NameplateVisibilityFacetPreset

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e8/NameplateVisibilityFacetPresetComponent.png/510px-NameplateVisibilityFacetPresetComponent.png)](https://wiki.resonite.com/File:NameplateVisibilityFacetPresetComponent.png) **Nameplate Visibility Facet Preset** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **NameplateVisibilityFacetPreset** component loads the Nameplate Visibility facet when it's not `_fullyLoaded`. It does this by loading the facet from the cloud, and using that loaded data to make the preset

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

used in the main dash. no need to be used by the user unless they are missing the Nameplate Visibility facet.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NameplateVisibilityFacetPreset&oldid=93693](https://wiki.resonite.com/index.php?title=Component:NameplateVisibilityFacetPreset&oldid=93693)"

Contents