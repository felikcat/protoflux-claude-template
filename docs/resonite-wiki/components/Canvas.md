# Component:Canvas

> Source: https://wiki.resonite.com/Component:Canvas

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8b/CanvasComponent.png/510px-CanvasComponent.png)](https://wiki.resonite.com/File:CanvasComponent.png) **Canvas** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Canvas** component is the starting point for anything based on [UIX](https://wiki.resonite.com/UIX "UIX"). It provides the bounds of the UI and controls how users can interact with it.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

When updating certain things on the canvas, you may need to duplicate the entire [Slot](https://wiki.resonite.com/Slot "Slot") to get the canvas (and any other UIX elements and slots under that canvas) to work again. The specifics for this canvas component that may need to force recalculation are as follows:

- DefaultCulling: Especially for rendering the back side of the canvas.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Size` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The dimensions of the canvas. At normal scale, this is equivalent to meters |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This makes this component only editable in [Edit Mode](https://wiki.resonite.com/Edit_Mode "Edit Mode") |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptExistingTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If this canvas is already being touched (physically or remotely), accept the input |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `IgnoreTouchesFromBehind` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes the canvas ignore all touches from behind |
| `BlockAllInteractions` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Prevents any interaction if enabled |
| `LaserPassThrough` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allows the laser to go through the canvas |
| `PixelScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Sets the pixel scale for this canvas and its contents |
| `UnitScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Scales the contents of this canvas, higher number makes the contents smaller |
| `_rootRect` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | Internal - The root rect of this canvas |
| `Collider` | **[BoxCollider](https://wiki.resonite.com/Component:BoxCollider "Component:BoxCollider")** | The collider that receives touches from this canvas |
| `DefaultCulling` | **[Culling](https://wiki.resonite.com/Type:Culling "Type:Culling")** | Culling for this canvas |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Internal - Takes in a box collider and uses it for the canvas |
| `_colliderOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Internal - Offsets this box collider for this canvas |
| `StartingOffset` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The visibility order of rendering this canvas (lower number gets drawn over higher numbers) |
| `StartingMaskDepth` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Masking layer for the canvas |

Fields
Collapse

## Usage

This component is needed for [UIX](https://wiki.resonite.com/UIX "UIX"), without it, your other components that relay on UIX, canvas, elements, and [rects](https://wiki.resonite.com/Type:Rect "Type:Rect") will not work as expected. Using a canvas not only organizes your other components, it renders them and makes them usable and interactable.

## Examples

Here is a video from [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")'s tutorial on canvases:

![](https://i.ytimg.com/vi/cLtD7uWrduI/hqdefault.jpg)

[OLD: Neos VR Tutorial: UIX Pt.1 Canvases and Rectangles](https://www.youtube-nocookie.com/embed/cLtD7uWrduI?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See also

- When a child slot is created when under a [Slot](https://wiki.resonite.com/Slot "Slot") that has a canvas component, the new child slot will automatically create a [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform") component.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Canvas&oldid=113558](https://wiki.resonite.com/index.php?title=Component:Canvas&oldid=113558)"

Contents