# Component:Camera

> Source: https://wiki.resonite.com/Component:Camera

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/20/CameraComponent.png/510px-CameraComponent.png)](https://wiki.resonite.com/File:CameraComponent.png) **Camera** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Camera** component represents a [Unity Camera](https://docs.unity3d.com/ScriptReference/Camera.html) which is centered on the slot and facing in the [forward direction](https://wiki.resonite.com/Coordinate_spaces#Directions "Coordinate spaces").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DoubleBuffered` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines if [DoubleBuffering](https://en.wikipedia.org/wiki/Multiple_buffering#Double_buffering_in_computer_graphics) is applied or not. |
| `ForwardOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determine whether the render technique is only forward. |
| `Projection` | **[CameraProjection](https://wiki.resonite.com/index.php?title=Type:CameraProjection&action=edit&redlink=1 "Type:CameraProjection (page does not exist)")** | Determines whether it's [perspective](https://en.wikipedia.org/wiki/Perspective_(graphical)) or [orthographic](https://en.wikipedia.org/wiki/Orthographic_projection) |
| `OrthographicSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size of the render-output in orthographic view. (Only active when `Projection` is set to `Orthographic` |
| `FieldOfView` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The vertical field of view of the camera. (Only active when `Projection` is set to `Perspective` |
| `NearClipping` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The point in meters where the camera ignores near objects. |
| `FarClipping` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The point in meters where the camera ignores far objects. |
| `UseTransformScale` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines if the scale of the camera should be taken into account. |
| `Clear` | **[CameraClearMode](https://wiki.resonite.com/Type:CameraClearMode "Type:CameraClearMode")** | See [Camera Clear Mode](https://wiki.resonite.com/Type:CameraClearMode "Type:CameraClearMode") for what this does. |
| `ClearColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | If `CameraClearMode` is set to `Color`. |
| `Viewport` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | 2D rectangular where the camera is allowed to render |
| `Depth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Whether this camera should be rendered before or after other cameras render. |
| `RenderTexture` | **[RenderTexture](https://wiki.resonite.com/Type:RenderTexture "Type:RenderTexture")** | The RenderTextureProvider input in order to get a ITexture2D |
| `Postprocessing` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines if post processing is allowed. |
| `ScreenSpaceReflections` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines if [ScreenSpaceReflections](https://en.wikipedia.org/wiki/Reflection_(computer_graphics)#Approaches_to_reflection_rendering) are rendered. |
| `MotionBlur` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines if MotionBlur is rendered or not. |
| `RenderShadows` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines if shadows are rendered or not. |
| `SelectiveRender` | _direct_ **[AutoSyncRefList\`1](https://wiki.resonite.com/index.php?title=Type:AutoSyncRefList%601&action=edit&redlink=1 "Type:AutoSyncRefList`1 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | A list of SyncReferences to slots the camera is allowed to render. |
| `ExcludeRender` | _direct_ **[AutoSyncRefList\`1](https://wiki.resonite.com/index.php?title=Type:AutoSyncRefList%601&action=edit&redlink=1 "Type:AutoSyncRefList`1 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | A list of SyncReferences to slots the camera is NOT allowed to render. |

Fields
Collapse

## Usage

Put the component onto a slot, and position the slot. The produced image can either be accesed through a [RenderTextureProvider](https://wiki.resonite.com/Component:RenderTextureProvider "Component:RenderTextureProvider") component or by creating a [Texture2D](https://wiki.resonite.com/Texture2D "Texture2D") asset using the [Render To Texture Asset](https://wiki.resonite.com/ProtoFlux:Render_To_Texture_Asset "ProtoFlux:Render To Texture Asset") Protoflux node.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

If a camera is connected to a [RenderTextureProvider](https://wiki.resonite.com/Component:RenderTextureProvider "Component:RenderTextureProvider"), it will flash its contents to the screen whenever any field of the RenderTextureProvider is changed. To work around this, be sure to set the `Depth` value on the Camera component to something below `0` if you plan to change any fields while it is active. See [this comment on issue #964 for more information.](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/964#issuecomment-2877264413)

## Examples

Security cameras, drones, picture takers, layered texture bakers, scanners, and more.

## See also

- [Component:CameraPortal](https://wiki.resonite.com/Component:CameraPortal "Component:CameraPortal"), which is often used as a mirror.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Camera&oldid=108572](https://wiki.resonite.com/index.php?title=Component:Camera&oldid=108572)"

Contents