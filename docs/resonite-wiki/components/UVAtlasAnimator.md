# Component:UVAtlasAnimator

> Source: https://wiki.resonite.com/Component:UVAtlasAnimator

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b9/UVAtlasAnimatorComponent.png/510px-UVAtlasAnimatorComponent.png)](https://wiki.resonite.com/File:UVAtlasAnimatorComponent.png) **UVAtlas Animator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UVAtlasAnimator** component is used primarily to drive texture animations on [materials](https://wiki.resonite.com/Material "Material") like GIFs. It can also be used as a sprite sheet to animate things like 2D mouths.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ScaleField` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The texture's `TextureScale` field that should be driven |
| `OffsetField` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The texture's `TextureOffset` field that should be driven |
| `AtlasInfo` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [AtlasInfo](https://wiki.resonite.com/Component:AtlasInfo "Component:AtlasInfo") >** | The [AtlasInfo](https://wiki.resonite.com/AtlasInfo_(Component) "AtlasInfo (Component)") component that provides the size and frame amount for the atlas |
| `Frame` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Which frame of the atlas the texture scale and offset should be driven to |

Fields
Collapse

## Usage

Attach to a slot and provide the component with the Scale and Offset fields of any [Material](https://wiki.resonite.com/Material "Material"). Then, set the material's image to a sprite sheet of a set of animation frames. Then provide a [Component:AtlasInfo](https://wiki.resonite.com/Component:AtlasInfo "Component:AtlasInfo") with the proper data. Finally, use a [Component:TimeIntDriver](https://wiki.resonite.com/Component:TimeIntDriver "Component:TimeIntDriver") to drive `Frame` to animate always, or set/drive `Frame` to the frame on the sheet you want in some other way like [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux").

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:AtlasInfo](https://wiki.resonite.com/Component:AtlasInfo "Component:AtlasInfo")
- [Component:TimeIntDriver](https://wiki.resonite.com/Component:TimeIntDriver "Component:TimeIntDriver")
- Component:UVAtlasAnimator

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UVAtlasAnimator&oldid=92343](https://wiki.resonite.com/index.php?title=Component:UVAtlasAnimator&oldid=92343)"

Contents