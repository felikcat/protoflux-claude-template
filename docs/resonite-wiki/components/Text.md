# Component:Text

> Source: https://wiki.resonite.com/Component:Text

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Text&diff=88654) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e7/TextComponent.png/510px-TextComponent.png)](https://wiki.resonite.com/File:TextComponent.png) **Text** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Text** component displays text inside of a [UIX](https://wiki.resonite.com/UIX "UIX") element. It also supports [text formatting](https://wiki.resonite.com/Text_Formatting "Text Formatting").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Font` | **[FontSet](https://wiki.resonite.com/Type:FontSet "Type:FontSet")** | The font to use |
| `Content` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | What [string](https://wiki.resonite.com/Type:String "Type:String") of text to display |
| `ParseRichText` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to interpret [text formatting](https://wiki.resonite.com/Text_Formatting "Text Formatting") |
| `NullContent` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | What to display if Content is empty |
| `Size` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size to render text at, in display units |
| `HorizontalAlign` | **[TextHorizontalAlignment](https://wiki.resonite.com/index.php?title=Type:TextHorizontalAlignment&action=edit&redlink=1 "Type:TextHorizontalAlignment (page does not exist)")** | How to align the text, horizontally |
| `VerticalAlign` | **[TextVerticalAlignment](https://wiki.resonite.com/index.php?title=Type:TextVerticalAlignment&action=edit&redlink=1 "Type:TextVerticalAlignment (page does not exist)")** | How to align the text, vertically |
| `AlignmentMode` | **[AlignmentMode](https://wiki.resonite.com/index.php?title=Type:AlignmentMode&action=edit&redlink=1 "Type:AlignmentMode (page does not exist)")** | How to compute alignment |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to render the text with |
| `Materials` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The Material(s) to render with |
| `LineHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How high each line of text is |
| `MaskPattern` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Text entered here will mask each character with this exact string (example for a password field: \*) |
| `HorizontalAutoSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Automatically adjusts the text's size to fit in its horizontal space |
| `VerticalAutoSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Automatically adjusts the text's size to fit in its vertical space |
| `AutoSizeMin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum size that can be reached via auto-sizing |
| `AutoSizeMax` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum size that can be reached via auto-sizing |
| `CaretPosition` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The text cursor position on this text |
| `SelectionStart` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The starting point for this text cursor |
| `CaretColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The text cursor color |
| `SelectionColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The text selection/highlight color |
| `InteractionTarget` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes this text as the interaction target for this UIX. |
| `_legacyFontMaterial` | **[FontMaterial](https://wiki.resonite.com/Component:FontMaterial "Component:FontMaterial")** | Internal |
| `_legacyAlign` | **[Alignment](https://wiki.resonite.com/index.php?title=Type:Alignment&action=edit&redlink=1 "Type:Alignment (page does not exist)")** | Internal |

Fields
Collapse

## Usage

Text can be used to explain something, to be descriptive, to notify, and many other things text can be used for. When being effective with text, basic graphic design principles apply even to something simple as text.

## Examples

Within the Resonite's Essential, there is an UI preset called the "Panel base". This UI preset uses the text component to display texts within the panel.

[![](https://wiki.resonite.com/images/thumb/e/e6/Text_component.jpg/800px-Text_component.jpg)](https://wiki.resonite.com/File:Text_component.jpg)

### Videos

Here is [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial on Text:

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Text&oldid=88654](https://wiki.resonite.com/index.php?title=Component:Text&oldid=88654)"

Contents