# Component:InteractionLaser

> Source: https://wiki.resonite.com/Component:InteractionLaser

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/de/InteractionLaserComponent.png/510px-InteractionLaserComponent.png)](https://wiki.resonite.com/File:InteractionLaserComponent.png) **Interaction Laser** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **InteractionLaser** component is part of the user to world interaction interfacing. This component is entirely regenerated separate from the avatar per respawn, making it un-reference-able.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to smooth laser movement for this laser. |
| `SmoothModulateStartAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Angle at which the laser smoothing speed will start modulating to catch up to your movements. Increasing this value will require larger movements for the laser to start catching up. |
| `SmoothModulateEndAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Related to the modulate start angle, this indicates when the modulation will reach maximum speed. By changing the start and end angles, you can control how responsive the laser is the more you move your hand. |
| `SmoothModulateExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls the response curve of the laser modulation between the start and end angles. You can use this to either make the laser respond more sluggishly at first or to start responding quickly and then tapering off. |
| `SmoothModulateMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The laser smoothing speed will be multiplied by this value once you have reached the modulate end angle. Increasing this value will make the laser catch up quicker once you move your hand far enough. Lowering the value will make it take longer to catch up. |
| `StickThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls how much the laser will stick to interactive items. Larger values will make it stick more. Setting this to zero will stop the stickiness completely. |
| `ShowInDesktop` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | When on, the laser visual will be rendered to you fully when in first person view in desktop mode. |
| `MaxTouchPenetrationDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determined by the [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource")'s `MaxTouchPenetrationDistance`. |
| `StickPointSpace` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot the laser is sticking to. |
| `StickPointPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position the laser is sticking to. |
| `_handler` | **[InteractionHandler](https://wiki.resonite.com/Component:InteractionHandler "Component:InteractionHandler")** | The interaction handler used to handle behavior for this component. |
| `_lastHit` | _direct_ **[AutoSyncRef\`1](https://wiki.resonite.com/index.php?title=Type:AutoSyncRef%601&action=edit&redlink=1 "Type:AutoSyncRef`1 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | The last slot hit by the laser. |
| `_lastInteractionTarget` | _direct_ **[AutoSyncRef\`1](https://wiki.resonite.com/index.php?title=Type:AutoSyncRef%601&action=edit&redlink=1 "Type:AutoSyncRef`1 (page does not exist)") < [IInteractionTarget](https://wiki.resonite.com/index.php?title=Type:IInteractionTarget&action=edit&redlink=1 "Type:IInteractionTarget (page does not exist)") >** | The last interactable element this laser hit. |
| `_lastInteractionModifier` | _direct_ **[AutoSyncRef\`1](https://wiki.resonite.com/index.php?title=Type:AutoSyncRef%601&action=edit&redlink=1 "Type:AutoSyncRef`1 (page does not exist)") < [ILaserInteractionModifier](https://wiki.resonite.com/index.php?title=Type:ILaserInteractionModifier&action=edit&redlink=1 "Type:ILaserInteractionModifier (page does not exist)") >** | The last interaction modifier this laser was affected by. |
| `_hitColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the laser should have when it hits something. |
| `_laserTextureSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed the texture of the laser moves for effects like dotted lines. |
| `_touchSource` | **[RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource")** | The touch source associated with this laser for touching things physically |
| `_laserMesh` | **[BentTubeMesh](https://wiki.resonite.com/Component:BentTubeMesh "Component:BentTubeMesh")** | The laser mesh being constantly updated to make up this laser's visual. |
| `_laserMaterial` | **[OverlayUnlitMaterial](https://wiki.resonite.com/index.php?title=OverlayUnlitMaterial&action=edit&redlink=1 "OverlayUnlitMaterial (page does not exist)")** | The material being used for this laser's visual. |
| `_laserTexture` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The texture being used for this laser's visual. |
| `_behindLaserTint` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The tint field being used for this laser's visual. |
| `_laserRenderQueue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The render queue field of the material being used for this laser's visual. |
| `_laserFrontTextureOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The front texture field of the material being used for this laser's visual. |
| `_laserBehindTextureOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The behind texture field of the material being used for this laser's visual. |
| `_directPoint` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field of the direct point of the bent tube mesh being used for this laser's visual. |
| `_actualPoint` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field of the actual point of the bent tube mesh being used for this laser's visual. |
| `_startColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field of the start color of the bent tube mesh being used for this laser's visual. |
| `_endColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field of the end color of the bent tube mesh being used for this laser's visual. |
| `_pointSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The field of the point slot of the bent tube mesh being used for this laser's visual. |
| `_pointSlotPos` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field of the position of the point slot being used for this laser's visual. |
| `_laserVisible` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field used to control the visibility of the laser. |
| `_cursorVisible` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field used to control the cursor visibility of the laser. |
| `_cursorRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the cursor visual. |
| `_cursorImageRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the cursor image visual. |
| `_cursorTexture` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The component used for the cursor texture. |
| `_cursorMaterial` | **[OverlayUnlitMaterial](https://wiki.resonite.com/index.php?title=OverlayUnlitMaterial&action=edit&redlink=1 "OverlayUnlitMaterial (page does not exist)")** | The material of the cursor. |
| `_cursorFrontTint` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field used to control the tint of the cursor when it is directly visible by the camera. |
| `_cursorBehindTint` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field used to control the tint of the cursor when it is not directly visible by the camera. |
| `_cursorRenderQueue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The render queue field of the material being used for this laser's cursor visual. |
| `_cursorOrientation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field used to control the orientation for this laser's cursor visual. |
| `_cursorTint` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field used to control the color for this laser's cursor visual. |
| `_directCursorVisualsVisible` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the cursor's direct view visuals are visible or not. |
| `_directCursorActive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | the field to drive with whether the direct cursor is active. |
| `_directCursorRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the direct cursor visual. |
| `_directCursorImageRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the direct cursor image. |
| `_directCursorOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the direct cursor's offset. |
| `_directCursorOrientation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive with the direct cursor's orientation. |
| `_directLineTarget` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive with the direct cursor's direct line position. |
| `_directLineMesh` | **[SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh")** | The mesh being used for the direct line visual. |
| `_segmentColorFront` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color field of the direct line mesh's front color. |
| `_segmentColorBehind` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color field of the direct line mesh's behind color. |
| `_segmentRenderQueue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The render queue field of the direct line mesh's material. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``GetTipPosition:Func`2<RelayTouchSource, Float3>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource"), [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | ✓ | Gets the tip position of this laser, keeping in mind the settings and values of the inputted [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource"). |
| ``GetTipDirection:Func`2<RelayTouchSource, Float3>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource"), [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | ✓ | Gets the tip direction of this laser, keeping in mind the settings and values of the inputted [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource"). |
| ``GetTouchType:Func`2<RelayTouchSource, TouchType>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource"), [TouchType](https://wiki.resonite.com/Type:TouchType "Type:TouchType") >** | ✓ | Gets the touch type of this laser, keeping in mind the settings and values of the inputted [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource"). |
| `GetTouchable:TouchableGetter` | **[TouchableGetter](https://wiki.resonite.com/index.php?title=Type:TouchableGetter&action=edit&redlink=1 "Type:TouchableGetter (page does not exist)")** | ✓ | Gets the touching status of an inputted [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource") and what it has touched if any. |

Triggers
Collapse

## Usage

Not to be interacted with by the user. handles internal behavior.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractionLaser&oldid=98929](https://wiki.resonite.com/index.php?title=Component:InteractionLaser&oldid=98929)"

Contents