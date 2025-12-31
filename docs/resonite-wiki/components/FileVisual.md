# Component:FileVisual

> Source: https://wiki.resonite.com/Component:FileVisual

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b0/FileVisualComponent.png/510px-FileVisualComponent.png)](https://wiki.resonite.com/File:FileVisualComponent.png) **File Visual** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FileVisual** component is used to handle the creation and interfacing with a file object, which is spawned into the world from inventory or using the "Raw" option when [Importing](https://wiki.resonite.com/Importing "Importing").

## Files

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MetadataSource` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [FileMetadata](https://wiki.resonite.com/Component:FileMetadata "Component:FileMetadata") >** | The component that handles importing and storing the file data this component is representing the visual of. |
| `TypeLabel` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The label that determines the file type/extension (aka the "png" part of "hello.png") |
| `NameLabel` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The name of the file before the extension (aka the "hello" part of "hello.png") |
| `FillMaterial` | **[PBS\_DualSidedMetallic](https://wiki.resonite.com/PBS_DualSidedMetallic "PBS DualSidedMetallic")** | The material being used for the file icon in the center. |
| `OutlineMaterial` | **[PBS\_DualSidedMetallic](https://wiki.resonite.com/PBS_DualSidedMetallic "PBS DualSidedMetallic")** | The material being used to outline the file icon. |
| `TypeMaterial` | **[PBS\_DualSidedMetallic](https://wiki.resonite.com/PBS_DualSidedMetallic "PBS DualSidedMetallic")** | The material being used to color the file type. this can be orange for models, and the color varies based on file type. |

Fields
Collapse

## Usage

Is used by the game to generate and handle the visuals of raw files. Is usually not directly utilized by the player.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

We need a picture of an imported raw file (what about the whats this.owo picture meme)

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FileVisual&oldid=93738](https://wiki.resonite.com/index.php?title=Component:FileVisual&oldid=93738)"

Contents