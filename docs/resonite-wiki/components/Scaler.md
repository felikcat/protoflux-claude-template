# Component:Scaler

> Source: https://wiki.resonite.com/Component:Scaler

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Scaler&diff=97718) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/cc/ScalerComponent.png/510px-ScalerComponent.png)](https://wiki.resonite.com/File:ScalerComponent.png) **Scaler** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Scaler** component scales a target scale based on the distance of the slot this component is on from ""Point"" = (`ScaleOffset` in `ScaleSource`'s transform space) with the distance of both points calculated in `ScaleSpace`.

If the slots are all under root, the `scaleTarget` is targeting the scale of this slot, `ScaleSource` is set to root, `ScaleMode` is set to 'FullIndependent', `ScaleOffest` is set to (0,0,0), `ScaleMultiplier` is set to (1,1,1), and the slot this component is on is an unmodified default cube, the edge of at least one part of the cube on this slot will match perfectly to Root.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ScaleOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset of point **A** to `ScaleSource`. |
| `ScaleMultiplier` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to multiply the strength of the distance from **A** to **B** after conversion has on scale. |
| `ScaleSource` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The source space of point **A**. |
| `ScaleMode` | **[Scaler.Mode](https://wiki.resonite.com/Component:Scaler#Mode)** | How to restrict the distance calculations for scaling certain axies. |
| `ScaleSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space to convert **A** and **B** to for distance measurement. |
| `scaleTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to the distance from **A** to **B** after conversion to space `ScaleSpace` and applying `ScaleMode` restrictions, and then muliplying by 2 \* `ScaleMultiplier`. |

Fields
Collapse

## Mode

| Name | Value | Description |
| --- | --- | --- |
| `FullUniform` | 0 | The distance calculation from point **A** to **B** should be equal on all axies. |
| `XYUniform` | 1 | The distance calculation from point **A** to **B** should be done between the XY plane and applied to X and Y axis equally before calculating Z distance separately. |
| `YZUniform` | 2 | The distance calculation from point **A** to **B** should be done between the YZ plane and applied to Y and Z axis equally before calculating X distance separately. |
| `XZUniform` | 3 | The distance calculation from point **A** to **B** should be done between the XZ plane and applied to X and Z axis equally before calculating Y distance separately. |
| `FullIndependent` | 4 | The distance calculation from point **A** to **B** should be done separately for each axis. |

Values

## Usage

Attach to a slot and fill the fields to start using this component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Scaler&oldid=97718](https://wiki.resonite.com/index.php?title=Component:Scaler&oldid=97718)"

Contents