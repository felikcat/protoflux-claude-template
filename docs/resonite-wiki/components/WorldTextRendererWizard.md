# Component:WorldTextRendererWizard

> Source: https://wiki.resonite.com/Component:WorldTextRendererWizard

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5e/WorldTextRendererWizardComponent.png/510px-WorldTextRendererWizardComponent.png)](https://wiki.resonite.com/File:WorldTextRendererWizardComponent.png) **World Text Renderer Wizard** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [World Text Renderer Wizard](https://wiki.resonite.com/index.php?title=World_Text_Renderer_Wizard&action=edit&redlink=1 "World Text Renderer Wizard (page does not exist)").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root to do processing for. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to replace text renderer materials with. |
| `Font` | **[FontSet](https://wiki.resonite.com/Type:FontSet "Type:FontSet")** | The font to override texts with. |
| `ProcessDisabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to process disabled texts or not. |
| `ProcessStandaloneRenderers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to process [Component:TextRenderers](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer"). |
| `ProcessUIXRenderers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to process [Component:Texts](https://wiki.resonite.com/Component:Text "Component:Text"). |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | What color to change the texts to. |
| `_tag` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | Only process texts with this tag. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetColor:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to change the color of all text under the target slot. |
| `ReplaceFont:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to change the font of all text under the target slot. |
| `ReplaceMaterial:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to change the material of all text under the target slot. |

Triggers
Collapse

## Usage

See [World Text Renderer Wizard](https://wiki.resonite.com/index.php?title=World_Text_Renderer_Wizard&action=edit&redlink=1 "World Text Renderer Wizard (page does not exist)").

## Examples

See [World Text Renderer Wizard](https://wiki.resonite.com/index.php?title=World_Text_Renderer_Wizard&action=edit&redlink=1 "World Text Renderer Wizard (page does not exist)").

## See Also

- [World Text Renderer Wizard](https://wiki.resonite.com/index.php?title=World_Text_Renderer_Wizard&action=edit&redlink=1 "World Text Renderer Wizard (page does not exist)")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldTextRendererWizard&oldid=100819](https://wiki.resonite.com/index.php?title=Component:WorldTextRendererWizard&oldid=100819)"

Contents