# Component:GridContainerPreset

> Source: https://wiki.resonite.com/Component:GridContainerPreset

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/85/GridContainerPresetComponent.png/510px-GridContainerPresetComponent.png)](https://wiki.resonite.com/File:GridContainerPresetComponent.png) **Grid Container Preset** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GridContainerPreset** component generates a [Component:GridContainerScreen](https://wiki.resonite.com/Component:GridContainerScreen "Component:GridContainerScreen") tab and set it up when not initialized before.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_initializer` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The C# Type of the object that initialized this preset. |
| `_initializedVersion` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The version that this preset initialized. Used to reinitialize the Grid Container Screen if it has new updates. |
| `_isModified` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the Grid Container Screen has new content like facets. |

Fields
Collapse

## Usage

Used to make automatically updating custom screens.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GridContainerPreset&oldid=96759](https://wiki.resonite.com/index.php?title=Component:GridContainerPreset&oldid=96759)"

Contents