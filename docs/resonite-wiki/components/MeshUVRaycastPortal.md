# Component:MeshUVRaycastPortal

> Source: https://wiki.resonite.com/Component:MeshUVRaycastPortal

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c2/MeshUVRaycastPortalComponent.png/510px-MeshUVRaycastPortalComponent.png)](https://wiki.resonite.com/File:MeshUVRaycastPortalComponent.png) **Mesh UVRaycast Portal** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component also known as a raycast portal allows users to interact with objects through a [camera](https://wiki.resonite.com/Component:Camera "Component:Camera").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Offset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far back from the camera's actual view direction to project from |
| `RayExit` | **[IUVToRayConverter](https://wiki.resonite.com/index.php?title=Type:IUVToRayConverter&action=edit&redlink=1 "Type:IUVToRayConverter (page does not exist)")** | Usually a [camera](https://wiki.resonite.com/Component:Camera "Component:Camera") |
| `UVOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The added offset to the UV point you hit on the mesh before it's projected out; best to keep this (0,0) unless needed |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The multiplied offset to the UV point you hit on the mesh before it's projected out; best to keep this (1,1) unless needed |
| `RepeatUV` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to repeat between the 0-1 range when the laser on the source hits a UV beyond 0-1 |
| `OverrideHitTriggers` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Whether to hit colliders, requires Filter to have a sync delegate, but doesn't need to be enabled for this component to work |
| `Filter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Func\`3](https://wiki.resonite.com/Type:Func%603 "Type:Func`3") < [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"), [Int](https://wiki.resonite.com/Type:Int "Type:Int"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | This is a field usually used by the dash manager in local space. Very hard to use, and is not required at all |
| `FilterMode` | **[FilterCombineMode](https://wiki.resonite.com/Type:FilterCombineMode "Type:FilterCombineMode")** | how to use the `Filter` if provided. |

Fields
Collapse

## Behavior

- The camera needs to be in orthographic mode for best results. it still works in perspective but because of perspective warping it only works well in the center. This component is used for the dash, but can be utilized in real world space, allowing for some interesting effects.

- This component only works with mesh colliders. The type of mesh does not matter, since it uses the UVs; the mesh triangles have to determine what point on the camera output to project the raycast out of.

- The mesh collider can only be a front sided collider for this component to work.

- Only user interaction lasers are allowed to pass through, and only press button interactions.

## Examples

In this example we will create a Camera, that looks at a Canvas, and a Quad that renders what the Camera sees.

The **MeshUVRaycastPortal** will transfer the laser interactions from the Quad's MeshCollider to the Canvas, through the Camera.

1\. Create New -> Object -> _Camera_

2\. Spawn -> `resdb:///613cb78341d5b330aee559a1871011ccfb733221428ff9601ce56e19c7b1631e.brson` ( I will refer to it as _Checkbox_)

- or from **Resonite Essentials** -\> Examples -> UIX -> _Checkbox_

3\. Place the _Checkbox_ in front of the _Camera_

4\. Create New -> 3D Model -> _Quad_

5\. Create New -> Materials -> PBS Metallic (for example)

6\. Set the Material as the Quad's Material

7\. Grab the _RenderTextureProvider_ from the _Camera_, and set it as this Material's MainTexture (AlbedoTexture)

8\. Inspect the _Quad_, and add the **MeshUVRaycastPortal**

9\. Set the **MeshUVRaycastPortal**'s Camera field to the _Camera_ created by us

10\. Now when you try to interact with the UI through the _Quad_, the UI should be responsive

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MeshUVRaycastPortal&oldid=113549](https://wiki.resonite.com/index.php?title=Component:MeshUVRaycastPortal&oldid=113549)"

Contents