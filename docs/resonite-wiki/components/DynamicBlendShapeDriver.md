# Component:DynamicBlendShapeDriver

> Source: https://wiki.resonite.com/Component:DynamicBlendShapeDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicBlendShapeDriver&diff=98439) which are not marked for translation.

This component is used to map values to Blendshapes by name.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d4/DynamicBlendShapeDriverComponent.png/510px-DynamicBlendShapeDriverComponent.png)](https://wiki.resonite.com/File:DynamicBlendShapeDriverComponent.png) **Dynamic Blend Shape Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Renderer` | **[SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer")** | The renderer to use to search for shapekeys with |
| `BlendShapes` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[DynamicBlendShapeDriver.BlendShape](https://wiki.resonite.com/Component:DynamicBlendShapeDriver#BlendShape)** | A list of [BlendShape](https://wiki.resonite.com/Component:DynamicBlendShapeDriver#BlendShape) that are searched for in order on the `Renderer`. |
| `_lastRenderer` | **[SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer")** | The last renderer that was searched. This value is automatically filled and is read only. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnUpdateBlendshapeTargets:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Trigger the filling of blendshapes in the `BlendShapes` list to the ones of the same names in `Renderer`. |

Triggers
Collapse

## BlendShape

| Name | Type | Description |
| --- | --- | --- |
| `Name` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the blendshape this subcomponent should look for to auto fill `Field` with |
| `Value` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | the value to drive `Field` to. |
| `Field` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | is usually auto filled with a blendshape's value on the `Renderer` that has a blendshape name matching `Name`. |

Fields

## Usage

To efficiently use this component, first add some blendshape items to the `blendshapes` list and give the blendshapes names of the blendshapes on your target mesh. Next, add the skinned mesh renderer to `Renderer` you want to automatically find the blendshapes for. The component in the next update will automatically add the value sliders of the blendshapes it can find on the target `Renderer` to the `Field` on each `BlendShape`.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

The fields will not all fill if it cannot find the blendshape for a `BlendShape`. The component will find the blendshapes in order of how they are listed in this component. If a blendshape cannot be found, the component will disable itself and not fill the drive. Either remove the `BlendShape` from the list of `BlendShapes` or fix the `Name` field of the offending `BlendShape`

To drive the blendshapes, just simply drive the `Value` on each `BlendShape` for each blendshape you want. Driving `Value` is not required, and this can be used in cases where you wanna toggle, cycle, or write with flux a blendshape's value without driving it. This can be useful if you don't wanna accidentally bake blendshapes you are still using despite them not being driven

## Examples

This component is useful for auto detecting blendshapes like expression drivers via systems. It is also useful for counteracting issues where adding blendshapes to an existing avatar will cause the blendshapes to change order in the array of blendshapes. Using this component allows for also automatically setting drives for blendshapes, without having references to them prior.

For example, putting a [Dynamic Reference Variable<SkinnedMeshRenderer>](https://wiki.resonite.com/Component:DynamicReferenceVariable "Component:DynamicReferenceVariable") for the mesh on an avatar for it's face, can allow for an external system to find the mmd blendshapes on a character using this component for mmd animations.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicBlendShapeDriver&oldid=98439](https://wiki.resonite.com/index.php?title=Component:DynamicBlendShapeDriver&oldid=98439)"

Contents