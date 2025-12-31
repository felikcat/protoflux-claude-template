# Component:SpriteProvider

> Source: https://wiki.resonite.com/Component:SpriteProvider

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SpriteProvider&diff=113514) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0b/SpriteProviderComponent.png/510px-SpriteProviderComponent.png)](https://wiki.resonite.com/File:SpriteProviderComponent.png) **SpriteProvider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A **SpriteProvider** defines a slice of a [Texture2D](https://wiki.resonite.com/Texture2D "Texture2D") as a [Sprite](https://wiki.resonite.com/Sprite "Sprite") that may be used by other components e.g. [UIX](https://wiki.resonite.com/UIX "UIX") [Images](https://wiki.resonite.com/Component:Image "Component:Image") to display graphics or produce backgrounds.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The sprite to provide. |
| `Rect` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The rectangle within the sprite to render. Note that the second x and y are actually the width and height of the Rect. The values are proportions of the width and height of the image in the Texture property. |
| `Borders` | **[Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4")** | Border widths for [9-slice scaling](https://wiki.resonite.com/9-slice_scaling "9-slice scaling"). The XYZW components set the left, bottom, right, and top borders respectively. |
| `Scale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Effects the center size when 9 slicing. |
| `FixedSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Effects the center size when 9 slicing. |

Fields
Collapse

## Behavior

Sprite providers due to the current Unity implementation at the time of writing this have issues with switching images very quickly. They will often flash white, causing a health hazard to photo sensitive users. Having all the sprites on UIX elements at once and switching their `OrderOffset` to change which element renders on top will remove the flashing and is currently the only way to combat this issue.

**Using SpriteProvider to break up a sprite-sheet of iconography:**

By combining multiple icons/elements in a grid-like texture, you can reduce the size of your objects and improve load performance by reusing the same texture for multiple sprites. Please note that the `Rect` values are floating point percentages of the texture were 1 would equal 100%, so 1/4 or 25% would be 0.25 in floating point value.

The `Rect` first x,y values are from the LOWER LEFT of the texture being 0.0, 0.0, where the total inclusion of the cut out texture sprite is a percentage of the width and height in the second x,y values.

Example: Given if you take a 1024x1024 px sprite sheet texture.

- Divide the height and width by 4 to make 12 equal sprite slots of 256x256 px chunks
- A sprite texture on the second column from the left and on the third row from the bottom would be `Rect`: x: 0.25 y: 0.50 x: 0.25 y: 0.25

See attached example diagram for help.

## Examples

[ProbablePrime's](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime") video on Sprites

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

[![caption](https://wiki.resonite.com/images/5/55/SpriteSheetDiagram.png)](https://wiki.resonite.com/File:SpriteSheetDiagram.png "caption")

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SpriteProvider&oldid=113514](https://wiki.resonite.com/index.php?title=Component:SpriteProvider&oldid=113514)"

Contents