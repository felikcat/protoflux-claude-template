# Component:ReflectionProbe

> Source: https://wiki.resonite.com/Component:ReflectionProbe

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fa/ReflectionProbeComponent.png/510px-ReflectionProbeComponent.png)](https://wiki.resonite.com/File:ReflectionProbeComponent.png) **Reflection Probe** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ReflectionProbe** component is used to make points in space that makes reflective surfaces within a box around the point show a different reflection map than the skybox. This is useful for controlling the lighting and look of a scene.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ProbeType` | **[ReflectionProbe.Type](https://wiki.resonite.com/Component:ReflectionProbe#Type)** | What mode this reflection probe uses. |
| `Importance` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How much priority this probe takes over another probe when two probes overlap |
| `Intensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how strong or bright the reflection is |
| `BlendDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how far the probe will slowly take over the reflection map of objects as an object goes towards the center of influence |
| `BoxSize` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the area that this reflection probe will affect the reflection maps of objects |
| `BoxProjection` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | project the reflection map in a box shape from the reflection probe rather than a sphere. |
| `BakedCubemap` | **[Cubemap](https://wiki.resonite.com/Type:Cubemap "Type:Cubemap")** | The cube map to replace the refection maps of reflective objects with in the influence area of this reflection probe |
| `ChangesSources` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IChangeable](https://wiki.resonite.com/index.php?title=Type:IChangeable&action=edit&redlink=1 "Type:IChangeable (page does not exist)") >** | A list of elements that will prompt this reflection probe to render a new map whenever they change. |
| `TimeSlicing` | **[ReflectionProbe.TimeSlicingMode](https://wiki.resonite.com/Component:ReflectionProbe#TimeSlicingMode)** | How updates to this reflection probe should happen in updates if this probe is a realtime probe. |
| `Resolution` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | the forced resolution of the reflection map from this reflection probe shown in the reflections of shiny objects. |
| `HDR` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the color encoding should be in HDR. |
| `ShadowDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how far to render shadows from the reflection probe |
| `ClearFlags` | **[ReflectionProbe.Clear](https://wiki.resonite.com/Component:ReflectionProbe#Clear)** | Whether to use the skybox or color when backing transparent pixels |
| `BackgroundColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to clear with when `ClearFlags` is set to "Color" |
| `NearClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The closest distance to render from the reflection probe center when using "Realtime" on `ProbeType` |
| `FarClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The furthest distance to render from the reflection probe center when using "Realtime" on `ProbeType` |
| `SkyboxOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to render only the skybox or not. |
| `ShowDebugVisuals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Shows the box influence area and the center point of this reflection probe |
| `_debugVisual` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | The current debug visual that this reflection probe is showing, if applicable. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnBake:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the bake button is touched. |
| `Bake:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Creates a static cubemap and inserts it into `BakedCubemap` instead of having `ProbeType` be set to realtime. |

Triggers
Collapse

## Type

| Name | Value | Description |
| --- | --- | --- |
| `Realtime` | 0 | render a new cube map outwards from the center of the probe every second |
| `OnChanges` | 1 | render a new cubemap every time one of the elements in `ChangesSources` changes. |
| `Baked` | 1 | use the provided `BakedCubemap` |

Values

## Clear

| Name | Value | Description |
| --- | --- | --- |
| `Skybox` | 0 | back transparent parts of the reflection map due to far or near clipping or transparent pixels in the provided `BakedCubemap` with the Skybox of the world. |
| `Color` | 1 | backs the transparent parts of the reflection map due to far or near clipping with realtime, or transparent pixels in the provided `BakedCubemap` with `BackgroundColor`. |

Values

## TimeSlicingMode

| Name | Value | Description |
| --- | --- | --- |
| `AllFacesAtOnce` | 0 | spreads update over 9 frames |
| `IndividualFaces` | 1 | spreads update over 14 frames |
| `NoTimeSlicing` | 2 | No time slicing should be applied to capturing. Update happens within one frame. |

Values

## Usage

Attach to a slot to start using this component as a point source for reflection map data.

## Examples

Can be used for real time lighting changes, or to create custom reflection maps in an area.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReflectionProbe&oldid=99158](https://wiki.resonite.com/index.php?title=Component:ReflectionProbe&oldid=99158)"

Contents