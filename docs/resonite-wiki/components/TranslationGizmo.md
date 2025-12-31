# Component:TranslationGizmo

> Source: https://wiki.resonite.com/Component:TranslationGizmo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b5/TranslationGizmoComponent.png/510px-TranslationGizmoComponent.png)](https://wiki.resonite.com/File:TranslationGizmoComponent.png) **Translation Gizmo** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Handles the translation of slots on the X, Y, Z directions or a combination thereof.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_xyzGizmo` | **[VolumeTranslationGizmo](https://wiki.resonite.com/Component:VolumeTranslationGizmo "Component:VolumeTranslationGizmo")** | The gizmo that allows translations on xyz at the same time. |
| `_xyGizmo` | **[PlaneTranslationGizmo](https://wiki.resonite.com/Component:PlaneTranslationGizmo "Component:PlaneTranslationGizmo")** | The gizmo that allows translations on xy at the same time. |
| `_xzGizmo` | **[PlaneTranslationGizmo](https://wiki.resonite.com/Component:PlaneTranslationGizmo "Component:PlaneTranslationGizmo")** | The gizmo that allows translations on xz at the same time. |
| `_yzGizmo` | **[PlaneTranslationGizmo](https://wiki.resonite.com/Component:PlaneTranslationGizmo "Component:PlaneTranslationGizmo")** | The gizmo that allows translations on yz at the same time. |
| `_xGizmo` | **[AxisTranslationGizmo](https://wiki.resonite.com/Component:AxisTranslationGizmo "Component:AxisTranslationGizmo")** | The gizmo that allows translation on x. |
| `_yGizmo` | **[AxisTranslationGizmo](https://wiki.resonite.com/Component:AxisTranslationGizmo "Component:AxisTranslationGizmo")** | The gizmo that allows translation on y. |
| `_zGizmo` | **[AxisTranslationGizmo](https://wiki.resonite.com/Component:AxisTranslationGizmo "Component:AxisTranslationGizmo")** | The gizmo that allows translation on z. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TranslationGizmo&oldid=106599](https://wiki.resonite.com/index.php?title=Component:TranslationGizmo&oldid=106599)"

Contents