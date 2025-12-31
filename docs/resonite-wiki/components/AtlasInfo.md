# Component:AtlasInfo

> Source: https://wiki.resonite.com/Component:AtlasInfo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/53/AtlasInfoComponent.png/510px-AtlasInfoComponent.png)](https://wiki.resonite.com/File:AtlasInfoComponent.png) **Atlas Info** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Atlas info is used in the [Component:UVAtlasAnimator](https://wiki.resonite.com/Component:UVAtlasAnimator "Component:UVAtlasAnimator") to provide the animator with information on format of an image that is an atlas of all the frames in an animation.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `GridSize` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The size of the grid that the image frames take up on the atlas (Ex: 4 by 8 grid of frames for a max of 32 total frames) |
| `GridFrames` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The amount of frames on the animation atlas image. If the amount of frames is less than the max (the two `GridSize` numbers multiplied together) then it will stop on frame `GridFrames` when this component is used by UVAtlasAnimator. |

Fields
Collapse

## Usage

When used in conjunction with a [TimeIntDriver](https://wiki.resonite.com/Component:TimeIntDriver "Component:TimeIntDriver"), and a [Component:UVAtlasAnimator](https://wiki.resonite.com/Component:UVAtlasAnimator "Component:UVAtlasAnimator") this can let you animate for example pixel art images (spritesheets, Atlases, etc)
AtlasInfo by itself dosen't have much use but when placed on a UVAtlasAnimator which is driving the Scale and Offset fields of a Material it will transform the UV of the material so that only one frame of the Texture is visible at a time

To automate the change of frames over time, you can use a [TimeIntDriver](https://wiki.resonite.com/index.php?title=TimeIntDriver&action=edit&redlink=1 "TimeIntDriver (page does not exist)") and set the repeat to Frames +1
Repeat field is \[0,x) \|\| \[0,x\]\
\
## Examples\
\
## See Also\
\
- Component:AtlasInfo\
- [Component:TimeIntDriver](https://wiki.resonite.com/Component:TimeIntDriver "Component:TimeIntDriver")\
- [Component:UVAtlasAnimator](https://wiki.resonite.com/Component:UVAtlasAnimator "Component:UVAtlasAnimator")\
\
Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AtlasInfo&oldid=97160](https://wiki.resonite.com/index.php?title=Component:AtlasInfo&oldid=97160)"\
\
Contents