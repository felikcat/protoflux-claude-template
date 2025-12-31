# Component:RadiantModalOverlay

> Source: https://wiki.resonite.com/Component:RadiantModalOverlay

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RadiantModalOverlay&diff=113376) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d8/RadiantModalOverlayComponent.png/510px-RadiantModalOverlayComponent.png)](https://wiki.resonite.com/File:RadiantModalOverlayComponent.png) **RadiantModalOverlay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RadiantModalOverlay** component is similar to the [ModalOverlay](https://wiki.resonite.com/Component:ModalOverlay "Component:ModalOverlay"), but with the [dash menu](https://wiki.resonite.com/Dash_menu "Dash menu"). This also can be duplicated as a template in the [ModalOverlayManager](https://wiki.resonite.com/Component:ModalOverlayManager "Component:ModalOverlayManager") component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ShowLerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The lerp amount for this modal. |
| `AnimationTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The lerp time for this modal. |
| `SizeRoot` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The size of this modal. |
| `ContentRoot` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The center root of this modal. |
| `CloseOnContextMenuAction` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Closes the modal when the user's context menu closes. |
| `CloseOnClick` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Closes this modal when it is clicked on. |
| `BlurSpread` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The blur effect amount. |
| `BackgroundColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The background color of this RadiantModalOverlay. |
| `ContentAnimationScaleOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Offests the content animation for this RadiantModalOverlay. |
| `HeaderSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The header size of this RadiantModalOverlay. |
| `Padding` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The padding amount for this RadiantModalOverlay. |
| `_title` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The title of this RadiantModalOverlay. |
| `_blur` | **[BlurMaterial](https://wiki.resonite.com/index.php?title=BlurMaterial&action=edit&redlink=1 "BlurMaterial (page does not exist)")** | The blur of this RadiantModalOverlay. |
| `_blurGraphic` | **[RawGraphic](https://wiki.resonite.com/Component:RawGraphic "Component:RawGraphic")** | The blur graphic of this RadiantModalOverlay. |
| `_blurSpread` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The blur speed of this RadiantModalOverlay. |
| `_backgroundColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The background color of this RadiantModalOverlay. |
| `_maskRect` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The mask rect of this RadiantModalOverlay. |
| `_headerOffsetMin` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The header offset min of this RadiantModalOverlay. |
| `_headerOffsetMax` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The header offset max of this RadiantModalOverlay. |
| `_contentOffsetMin` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The content offset min of this RadiantModalOverlay. |
| `_contentOffsetMax` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The content offset max of this RadiantModalOverlay. |
| `_titleOffsetMin` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The title offset min of this RadiantModalOverlay. |
| `_titleOffsetMax` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The title offset max of this RadiantModalOverlay. |
| `_closeOffsetMin` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The close offset min of this RadiantModalOverlay. |
| `_closeOffsetMax` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The close offset max of this RadiantModalOverlay. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `DoClose:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when this UI is closed. |

Triggers
Collapse

## Usage

## Examples

## See Also

- [Component:ModalOverlay](https://wiki.resonite.com/Component:ModalOverlay "Component:ModalOverlay")
- [Component:ModalOverlayManager](https://wiki.resonite.com/Component:ModalOverlayManager "Component:ModalOverlayManager")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RadiantModalOverlay&oldid=113376](https://wiki.resonite.com/index.php?title=Component:RadiantModalOverlay&oldid=113376)"

Contents