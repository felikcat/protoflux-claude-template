# Component:OrientAtPoint

> Source: https://wiki.resonite.com/Component:OrientAtPoint

Collapse **Component image**

[File:OrientAtPointComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=OrientAtPointComponent.png "File:OrientAtPointComponent.png") **Orient At Point** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Orient At Point** component makes particles in a particle system orient at a point in a specified transform space.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PointSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The tranform space `TargetPoint` and `Up` are in. |
| `TargetPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The point that particles should point at. |
| `Up` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction that should be up locally for each particle. |

Fields
Collapse

## Usage

used with [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") systems.

## Examples

## See Also

- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OrientAtPoint&oldid=101121](https://wiki.resonite.com/index.php?title=Component:OrientAtPoint&oldid=101121)"

Contents