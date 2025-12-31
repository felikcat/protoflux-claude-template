# Component:DataPresetReference

> Source: https://wiki.resonite.com/Component:DataPresetReference

Data Preset reference is a component that takes any reference type for PresetReference. When this is triggered by a [DataPreset](https://wiki.resonite.com/Component:DataPreset "Component:DataPreset"), this sets `TargetReference` to `PresetReference`.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/ce/DataPresetReference%601Component.png/510px-DataPresetReference%601Component.png)](https://wiki.resonite.com/File:DataPresetReference%601Component.png) **Data Preset Reference\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PresetReference` | **T** | The field reference for the preset. Since this is a generic component, it can be used with any type of reference. |
| `TargetReference` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T>>** | A reference to the reference field of the same type as PresetReference. |

Fields
Collapse

## Usage

See [DataPreset](https://wiki.resonite.com/Component:DataPreset "Component:DataPreset") for usage.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DataPresetReference&oldid=93383](https://wiki.resonite.com/index.php?title=Component:DataPresetReference&oldid=93383)"

Contents