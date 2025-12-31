# Component:DataPresetValue

> Source: https://wiki.resonite.com/Component:DataPresetValue

Data Preset reference is a component that takes any value type for PresetValue. When this is triggered by a [DataPreset](https://wiki.resonite.com/Component:DataPreset "Component:DataPreset"), this sets `TargetField` to `PresetValue`.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b9/DataPresetValue%601Component.png/510px-DataPresetValue%601Component.png)](https://wiki.resonite.com/File:DataPresetValue%601Component.png) **Data Preset Value\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PresetValue` | **T** | The value for the preset. Float is used as an example. Since this is a generic component, it can be used with any value. |
| `TargetField` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | A reference to the field of the same type as PresetValue. |

Fields
Collapse

## Usage

See [DataPreset](https://wiki.resonite.com/DataPreset_(Component) "DataPreset (Component)") for usage.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DataPresetValue&oldid=82637](https://wiki.resonite.com/index.php?title=Component:DataPresetValue&oldid=82637)"

Contents