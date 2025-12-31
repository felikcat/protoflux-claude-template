# Component:BoxBrushTool

> Source: https://wiki.resonite.com/Component:BoxBrushTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d6/BoxBrushToolComponent.png/510px-BoxBrushToolComponent.png)](https://wiki.resonite.com/File:BoxBrushToolComponent.png) **Box Brush Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BoxBrushTool** component is a tool that draws clouds of rotated, scaled, and UV mapped boxes as part of a [Component:BoxArrayMesh](https://wiki.resonite.com/Component:BoxArrayMesh "Component:BoxArrayMesh").

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
| `StrokePointRate` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | A multiplier to the affect of speed on the generation of points, so point generation is more concentrated over distance. |
| `ConstantPointRate` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | A multiplier for the point generation rate while drawing |
| `PressureAffectsRate` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether tool pressure affects point generation rate |
| `PressureAffectsRadius` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether tool pressure effects the radius around the brush tip that points are generated. |
| `ParticleSpawnRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius from the brush tip that points are generated including for particles |
| `SnapPoints` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether generated points should snap to snappers like snapping planes, circles, lines, etc |
| `Pivot` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset of the rotation Pivot of each box. |
| `MinColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The min color that each box can be. |
| `MaxColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The max color that each box can be. |
| `ColorGap` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the bias for the random colors for boxes. |
| `UniformSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether all boxes should be the same size always. |
| `MinSize` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the min size a drawn box can be. |
| `MaxSize` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the max size a drawn box can be. |
| `SizeGap` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the bias for the random size for boxes. |
| `MinRotation` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the minimum rotation of each box. |
| `MaxRotation` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the maximum rotation of each box. |
| `MinUVScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the minimum UV scale of each box. |
| `MaxUVScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the maximum uv scale of each box. |
| `UVScaleGap` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the bias of the uv scale of each box. |
| `RotationSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The transform space that should be used when applying rotation to the boxes. |
| `UseColor` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the boxes should have vertex colors. |
| `ScaleUVWithSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether boxes should have more UV detail the bigger they are. |
| `_previewRenderer` | **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | The renderer being used to render the mesh preview of this brush. |
| `_previewMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[BoxArrayMesh](https://wiki.resonite.com/Component:BoxArrayMesh "Component:BoxArrayMesh")** | The mesh being used to preview the stroke of this brush. |
| `_previewMeshOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position offset of the mesh preview for this brush. |
| `_previewMeshRotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the preview mesh. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``ChangeSize:Action`1<Float>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | ✓ | Handles changing the size of the brush of a brush tool. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxBrushTool&oldid=98335](https://wiki.resonite.com/index.php?title=Component:BoxBrushTool&oldid=98335)"

Contents