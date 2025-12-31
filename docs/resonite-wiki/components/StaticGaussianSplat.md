# Component:StaticGaussianSplat

> Source: https://wiki.resonite.com/Component:StaticGaussianSplat

Collapse **Component image**

[File:StaticGaussianSplatComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=StaticGaussianSplatComponent.png "File:StaticGaussianSplatComponent.png") **Static Gaussian Splat** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Static Gaussian Splat** component stores data for the [Gaussian Splat](https://wiki.resonite.com/Gaussian_Splat "Gaussian Splat") asset itself.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The location of the Gaussian Splat data. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``ClipWithBoundingBox:Func`2<BoundingBox, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Cuts the Gaussian splat using a bounding box argument. |
| ``ClipWithBoundingBox:Func`3<BoundingBox, FloatQ, Task`1<Bool>>`` | **[Func\`3](https://wiki.resonite.com/Type:Func%603 "Type:Func`3") < [BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox"), [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Cuts the Gaussian splat using a bounding box with rotation argument. |
| ``ClipWithSphere:Func`3<Float3, Float, Task`1<Bool>>`` | **[Func\`3](https://wiki.resonite.com/Type:Func%603 "Type:Func`3") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"), [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Cuts the Gaussian splat using a sphere argument. |
| `ColorByIndex:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Colors the Gaussian splat by index. |
| `ReoderMorton:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Reorders the splats using morton ordering. Which means any splats that are spatially near each other will also be near each other in the data indexes. |

Triggers
Collapse

## Usage

Used in Gaussian splat rendering components such as the [GaussianSplatRenderer](https://wiki.resonite.com/Component:GaussianSplatRenderer "Component:GaussianSplatRenderer") component.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StaticGaussianSplat&oldid=113570](https://wiki.resonite.com/index.php?title=Component:StaticGaussianSplat&oldid=113570)"

Contents