# Component:GeometryLineBrushTool

> Source: https://wiki.resonite.com/Component:GeometryLineBrushTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2c/GeometryLineBrushToolComponent.png/510px-GeometryLineBrushToolComponent.png)](https://wiki.resonite.com/File:GeometryLineBrushToolComponent.png) **Geometry Line Brush Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GeometryLineBrushTool** component is further explained on the
[Geometry Line Brush](https://wiki.resonite.com/Geometry_Line_Brush "Geometry Line Brush") page.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_equipLink` | _direct_ **[LinkTarget\`1](https://wiki.resonite.com/index.php?title=Type:LinkTarget%601&action=edit&redlink=1 "Type:LinkTarget`1 (page does not exist)") < [ITool](https://wiki.resonite.com/Type:ITool "Type:ITool") >** | This is Internal, and is used by the engine to retrieve the component this field is a part of. It cannot be assigned to. |
| `TipReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to use as the tool's tip, instead of the component's slot. |
| `BlockGripEquip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to prevent legacy double grip equipping from equipping this tooltip. |
| `BlockRemoteEquip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to prevent equipping by clicking via laser |
| `EquipName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the tool in the context menu when equipping via context menu. |
| `_overrideActiveTool` | **[InteractionHandler](https://wiki.resonite.com/Component:InteractionHandler "Component:InteractionHandler")** | The interaction handler to use instead of this tool as an interaction handler. |
| `_gripPosesGenerated` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the [Grip Pose Reference](https://wiki.resonite.com/Component:GripPoseReference "Component:GripPoseReference") components and slots have been generated for this tool. |
| `FixedMinimumPointDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Stroke point distances within a stroke cannot be less than this value. |
| `PositionSmoothing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to smooth the brush tip position when drawing. |
| `RotationSmoothing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to smooth the rotation of the brush tip when drawing |
| `PressureSmoothing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to smooth the brush pressure being applied |
| `MaxStrokeLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The longest a Brush stroke can be before being ended forcibly. |
| `StrokeFadeInLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The length along the stroke that the stroke fades in. |
| `StrokeFadeOutLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The length along the stroke that the stroke fades out. |
| `StrokeGroupFinishWaitTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Finishes the group when drawing strokes for more than this many seconds regardless of how full the group is. |
| `ActivationThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | When pressure/strength is above this value, the tool starts drawing. |
| `DeactivationThresholdRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | When pressure/strength is below this value, the tool stops drawing. |
| `MenuSizeChange` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to increment or decrement the brush size when using the context menu controls. |
| `SnapTip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the brush tip should snap to snappers like planes or snap spheres. |
| `SnapLine` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to snap new lines to snappers like snap planes or snap spheres. |
| `StrokesSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space to create new strokes into. |
| `MakeStrokesGrabbable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Make new strokes grabbable. |
| `PositionStrokesToTip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Position the slots of new stroke groups to the brush tip. |
| `OrientStrokesToTip` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Make the rotation of new stroke group slots oriented to the brush tip. |
| `ScaleStrokesToUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the brush strokes should be scaled up or down to match the user's scale. |
| `PickMaterials` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this brush can pick a material by dipping the brush tip in a material orb. |
| `PickColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this tool can pick colors by dipping the brush tip into a material orb. |
| `CurrentMaterial` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The current material the brush is using to draw. |
| `ColorMappings` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ColorMapping](https://wiki.resonite.com/index.php?title=Type:ColorMapping&action=edit&redlink=1 "Type:ColorMapping (page does not exist)")** | Associates materials with their color fields. |
| `ParticleSystem` | **[ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")** | The Particle system to Template when making Particle strokes. |
| `MeshEmitterTemplate` | **[MeshEmitter](https://wiki.resonite.com/Component:MeshEmitter "Component:MeshEmitter")** | The template component to use as the mesh emitter of new particle emitting strokes. |
| `ParticleTemplateHandling` | **[TemplateHandling](https://wiki.resonite.com/index.php?title=Type:TemplateHandling&action=edit&redlink=1 "Type:TemplateHandling (page does not exist)")** | How to handle the use of the Particle system template per new stroke group. |
| `EmissionRatePerUnitLength` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The rate of particle emission per unit length section of the stroke mesh. |
| `_colorPicker` | _direct_ **[SlotCleanupRef\`1](https://wiki.resonite.com/index.php?title=Type:SlotCleanupRef%601&action=edit&redlink=1 "Type:SlotCleanupRef`1 (page does not exist)") < [ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface") >** | The current color picker dialouge being used to pick a color for this brush. |
| `_pickedColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color that the tool has picked by being dipped in a material orb or picked via a color picker. |
| `_hideOnStroke` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The list of slots to hide while making a Brush stroke. |
| `_lastUsedMaterial` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The last used material by this brush. |
| `_lastCreatedMaterial` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The last material generated by this brush. |
| `Pressure` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The pressure being applied to the brush. |
| `Position` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the brush tip after smoothing. |
| `Rotation` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of the brush tip after smoothing. |
| `LastPointDelta` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The difference between the last drawing position and its current position. |
| `Velocity` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The velocity of the tool tips position. |
| `RawDelta` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The raw delta of the tool tips position. |
| `RawVelocity` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The raw velocity of the tool tip. |
| `RawStrokeLength` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The raw stroke length. |
| `StrokeLength` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The current stroke length in meters in `StrokesSpace` |
| `NormalizedStrokeLength` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The length of the current stroke from 0->1 where one is maximum length set for this brush for strokes. |
| `StrokeFadeMultiplier` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The multiplier to the fade in and out effects of the stroke. Making the fade in and out sharper or more gradual. |
| `StrokeGroupIndex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The running index of strokes being drawn as part of a stroke group. |
| `TipAnchor` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot used as the source of strokes being drawn. |
| `LineStyles` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[GeometryLineBrushTool.Line](https://wiki.resonite.com/Component:GeometryLineBrushTool#Line)** | A list of line styles this tool can possibly draw. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | the color profile of lines drawn by this tool. |
| `UseRelativeMinimumPointDistance` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | disable the size of the previous line size affecting minimum point distance. |
| `RelativeMinimumPointDistanceRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much size affects the minimum distance allowed between points. Affects how if a segment is bigger, that the next point has a bigger minimum place distance from that point. |
| `PressureAffectsSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether tool pressure affects line size. |
| `MaterialPreviews` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | A list of renderers showing previews of materials. |
| `_previewMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[MultiLineMesh](https://wiki.resonite.com/Component:MultiLineMesh "Component:MultiLineMesh")** | The mesh being used to preview the stroke of this brush. |
| `_previewMeshOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position offset of the mesh preview for this brush. |
| `_sizeKnob` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot being used as a size selector knob for this brush. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``ChangeSize:Action`1<Float>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | ✓ | Handles changing the size of the brush of a brush tool. |

Triggers
Collapse

## Line

| Name | Type | Description |
| --- | --- | --- |
| `Topology` | **[Topology](https://wiki.resonite.com/index.php?title=Type:Topology&action=edit&redlink=1 "Type:Topology (page does not exist)")** | The kind of Topology the line should have. |
| `Ends` | **[Ends](https://wiki.resonite.com/Type:Ends "Type:Ends")** | How the beginning and the ends of the line should be capped. |
| `Shading` | **[Shading](https://wiki.resonite.com/Type:Shading "Type:Shading")** | how the lines should be shaded. |
| `Points` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many divisions the line should have circumference wise. |
| `DualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the line should be dual sided. |
| `AbsolutePointOffsets` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the points in the line are absolute rather than offsets from the previous point. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the scale of the UVs of the line. |
| `ScaleUVByCircumference` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the detail per square unit should not change when the line has a bigger circumference. |
| `PreciseUV` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the UV for each line should be precise. |
| `PointOffsets` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the points of the line. |
| `ColorMode` | **[LineColorMode](https://wiki.resonite.com/Type:LineColorMode "Type:LineColorMode")** | How to apply `Color` for this line. |
| `Color` | **[Color](https://wiki.resonite.com/Type:Color "Type:Color")** | The vertex color for the vertices of this line. |
| `UseTipRotation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this line should be affected by Tool tip rotation. |
| `MaxSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The max radius this line can be at any given point. |
| `OverrideTip` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to use as an override when drawing this line. |
| `OverrideTipRotation` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot to use as a rotation override when drawing this line. |
| `OffsetSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space to put `PointOffsets` in for this line. |
| `RotationSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The space to use when applying rotation to this line. |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GeometryLineBrushTool&oldid=98395](https://wiki.resonite.com/index.php?title=Component:GeometryLineBrushTool&oldid=98395)"

Contents