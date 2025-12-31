# Component:RadiantDashProjectionMapper

> Source: https://wiki.resonite.com/Component:RadiantDashProjectionMapper

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8f/RadiantDashProjectionMapperComponent.png/510px-RadiantDashProjectionMapperComponent.png)](https://wiki.resonite.com/File:RadiantDashProjectionMapperComponent.png) **Radiant Dash Projection Mapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Dash menu](https://wiki.resonite.com/Dash_menu "Dash menu").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Dash` | **[RadiantDash](https://wiki.resonite.com/Component:RadiantDash "Component:RadiantDash")** | The Dash this is pointing to. |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the thing this is trying to project from. |
| `Mesh` | **[CurvedPlaneMesh](https://wiki.resonite.com/Component:CurvedPlaneMesh "Component:CurvedPlaneMesh")** | The mesh this is trying to project to. |
| `Camera` | **[Camera](https://wiki.resonite.com/Component:Camera "Component:Camera")** | The camera that is rendering `Root`. |
| `UVScale` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The scale field to drive in order to do the remapping. |
| `UVOffset` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The offset field to drive in order to do the remapping. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RadiantDashProjectionMapper&oldid=106533](https://wiki.resonite.com/index.php?title=Component:RadiantDashProjectionMapper&oldid=106533)"

Contents