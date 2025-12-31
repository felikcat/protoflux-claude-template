# Component:ScaleObjectCreator

> Source: https://wiki.resonite.com/Component:ScaleObjectCreator

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ScaleObjectCreator&diff=99164) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/23/ScaleObjectCreatorComponent.png/510px-ScaleObjectCreatorComponent.png)](https://wiki.resonite.com/File:ScaleObjectCreatorComponent.png) **Scale Object Creator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Manager` | **[ScaleObjectManager](https://wiki.resonite.com/Component:ScaleObjectManager "Component:ScaleObjectManager")** |  |
| `Template` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** |  |
| `TemplateNameField` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** |  |
| `TemplateSizeField` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Double](https://wiki.resonite.com/Type:Double "Type:Double") >** |  |
| `_sizeParser` | **[QuantityTextEditorParser\`1](https://wiki.resonite.com/Component:QuantityTextEditorParser%601 "Component:QuantityTextEditorParser`1") < [Distance](https://wiki.resonite.com/Type:Distance "Type:Distance") >** |  |
| `_material` | **[FresnelMaterial](https://wiki.resonite.com/Component:FresnelMaterial "Component:FresnelMaterial")** |  |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnAlign:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the align button is touched. |
| `OnCreate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the create item button is touched. |

Triggers
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScaleObjectCreator&oldid=99164](https://wiki.resonite.com/index.php?title=Component:ScaleObjectCreator&oldid=99164)"

Contents