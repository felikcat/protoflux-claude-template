# Component:TextureRefEditor

> Source: https://wiki.resonite.com/Component:TextureRefEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/10/TextureRefEditorComponent.png/510px-TextureRefEditorComponent.png)](https://wiki.resonite.com/File:TextureRefEditorComponent.png) **Texture Ref Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TextureRefEditor** component is commonly used in inspectors for materials and other components that use images/textures.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_targetRef` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") >>** | The field to make a visual for. |
| `_drive` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") >** | The field to drive with the contents of `_targetRef` or a placeholder texture if null. |
| `_clearReferenceButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to clear `_targetRef` |
| `_openInspectorButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to open an inspector for `_targetRef`. |
| `_copyTextureButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to copy the texture in `_targetRef`. |
| `_pasteTextureButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to paste a texture into `_targetRef`. |
| `_referenceText` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to drive with the description of the contents of `_targetRef`. |
| `_infoText` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to drive with the info of `_targetRef`. |
| `_isNormalMap` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `_targetRef` should be interpreted as a normal map. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `ClearReference:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the reference `_targetRef` is cleared via the UI button. |
| `OpenInspectorButton:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when an inspector is asked to be opened through this component for `_targetRef`. |
| `CopyTexture:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when a copy texture is called through this component for `_targetRef`. |
| `PasteTexture:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the user asks to paste a texture into `_targetRef` through this component. |
| `SetTexture:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the texture for `_targetRef` is set through this component. |

Triggers
Collapse

## Usage

Commonly used in inspectors. Using inspector specific components is a common tactic in [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking").

## Examples

Material inspector views.

## See Also

- [Ref Hacking](https://wiki.resonite.com/Ref_Hacking "Ref Hacking")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextureRefEditor&oldid=100743](https://wiki.resonite.com/index.php?title=Component:TextureRefEditor&oldid=100743)"

Contents