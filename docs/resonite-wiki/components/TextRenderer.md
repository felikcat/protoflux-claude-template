# Component:TextRenderer

> Source: https://wiki.resonite.com/Component:TextRenderer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/dd/TextRendererComponent.png/510px-TextRendererComponent.png)](https://wiki.resonite.com/File:TextRendererComponent.png) **Text Renderer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

The **TextRenderer** component shows Text in the world. An example can be created from the [Create New](https://wiki.resonite.com/Create_New_Wizard "Create New Wizard") menu, Text, then Basic or Outline.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `OverrideBoundingBox` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Force the bounding box calculated from this component to use `OverridenBoundingBox` instead of calculating when requested. |
| `OverridenBoundingBox` | **[BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox")** | the bounding box this component should say it has when `OverrideBoundingBox` is enabled. Useful for bounding box calculations with Flux, or changing the selection box for this component when rendered. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The profile that the vertex colors for this mesh should be displayed in. |
| `Font` | **[FontSet](https://wiki.resonite.com/Type:FontSet "Type:FontSet")** | The font set to use to render the text. For example, Times new Roman, or Avali Scratch. |
| `Text` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text to display. For example, "Hello world!" |
| `ParseRichText` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to interpret [text formatting](https://wiki.resonite.com/Text_Formatting "Text Formatting") tags like "<b></b>" for bold and "<i></i>" for itallic. |
| `NullText` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | the text to display if `Text` is null. (Empty text doesn't count) |
| `Size` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how big to render the text as. |
| `HorizontalAlign` | **[TextHorizontalAlignment](https://wiki.resonite.com/index.php?title=Type:TextHorizontalAlignment&action=edit&redlink=1 "Type:TextHorizontalAlignment (page does not exist)")** | How to align the text horizontally. |
| `VerticalAlign` | **[TextVerticalAlignment](https://wiki.resonite.com/index.php?title=Type:TextVerticalAlignment&action=edit&redlink=1 "Type:TextVerticalAlignment (page does not exist)")** | how to align the text vertically. |
| `AlignmentMode` | **[AlignmentMode](https://wiki.resonite.com/index.php?title=Type:AlignmentMode&action=edit&redlink=1 "Type:AlignmentMode (page does not exist)")** | how to align the text within the bounding box |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | what color to render the text in. |
| `Materials` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | what materials to render the text as. Really only works with [Unlit Text Material](https://wiki.resonite.com/Component:TextUnlitMaterial "Component:TextUnlitMaterial") type. |
| `LineHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much space each text line should take up |
| `Bounded` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to restrict the text within a certain area |
| `BoundsSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the area to use if `Bounded` is enabled. |
| `BoundsAlignment` | **[Alignment](https://wiki.resonite.com/index.php?title=Type:Alignment&action=edit&redlink=1 "Type:Alignment (page does not exist)")** | how to align the text to the bounds and therefore how to handle text that spills out. |
| `MaskPattern` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | a string to replace every character in `Text` with when rendering. Useful for password fields. |
| `HorizontalAutoSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to scale the text to fit the bounds horizontally |
| `VerticalAutoSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to scale the text to fit the bounds vertically |
| `CaretPosition` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Where the typing cursor position is within the text by character index. |
| `SelectionStart` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | where the selection starts if the text is being edited currently. |
| `CaretColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | the color of the typing cursor |
| `SelectionColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | the color of the typing selection. |
| `_legacyFontMaterial` | **[FontMaterial](https://wiki.resonite.com/Component:FontMaterial "Component:FontMaterial")** | Internal. |
| `_legacyAlign` | **[Alignment](https://wiki.resonite.com/index.php?title=Type:Alignment&action=edit&redlink=1 "Type:Alignment (page does not exist)")** | Internal. |

Fields
Collapse

## Sync delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Behavior

## Examples

Used in the "Basic" and "Outlined" text objects in the create new menu using a [Dev Tool](https://wiki.resonite.com/Dev_Tool "Dev Tool"). It's also useful in making physical UI's, and for signs. Anything generally text related that can be simple.

## See also

[UIX Text](https://wiki.resonite.com/Component:Text "Component:Text")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TextRenderer&oldid=108404](https://wiki.resonite.com/index.php?title=Component:TextRenderer&oldid=108404)"

Contents