# Component:RadiantDash

> Source: https://wiki.resonite.com/Component:RadiantDash

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/80/RadiantDashComponent.png/510px-RadiantDashComponent.png)](https://wiki.resonite.com/File:RadiantDashComponent.png) **Radiant Dash** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

**RadiantDash** controls the opening and closing animations of the [dash menu](https://wiki.resonite.com/Dash_menu "Dash menu"). When this component is created, it automatically creates child slots and the components it references.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `CurrentScreen` | **[RadiantDashScreen](https://wiki.resonite.com/Component:RadiantDashScreen "Component:RadiantDashScreen")** | The current screen this is showing. |
| `Open` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the dash is open. |
| `AnimationSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the dash should open and close. Equal to the reciprocal of the duration in seconds. (With the default value of 1.333..., opening and closing takes 0.75 seconds.) |
| `ScreenProjection` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this should be rendering in desktop mode. |
| `Curvature` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How curved the dash is. |
| `AspectRatioCompensation` | **[CurvedPlaneMesh.CurvatureAspectRatioCompensation](https://wiki.resonite.com/Component:CurvedPlaneMesh#CurvatureAspectRatioCompensation "Component:CurvedPlaneMesh")** | How much to compensate the animation for curvature |
| `ScreenSwitchingEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow user screen switching. |
| `_screensContainer` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to store different screens. |
| `_camera` | **[Camera](https://wiki.resonite.com/Component:Camera "Component:Camera")** | The camera being used to render the screen onto the curved surface. |
| `_renderTexture` | **[RenderTextureProvider](https://wiki.resonite.com/Component:RenderTextureProvider "Component:RenderTextureProvider")** | the texture to render to the curved surface. |
| `_topContainer` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to store top elements. |
| `_topMesh` | **[CurvedPlaneMesh](https://wiki.resonite.com/Component:CurvedPlaneMesh "Component:CurvedPlaneMesh")** | The mesh to show the top elements. |
| `_screenMesh` | **[CurvedPlaneMesh](https://wiki.resonite.com/Component:CurvedPlaneMesh "Component:CurvedPlaneMesh")** | The mesh to show the screen elements. |
| `_buttonsMesh` | **[CurvedPlaneMesh](https://wiki.resonite.com/Component:CurvedPlaneMesh "Component:CurvedPlaneMesh")** | The mesh to show the button elements. |
| `_topMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | The material to use for the top element. |
| `_screenMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | The material to use for the screen element. |
| `_buttonsMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | The material to use for the buttons element. |
| `_overlayEffectMaterial` | **[UI\_UnlitMaterial](https://wiki.resonite.com/Component:UI_UnlitMaterial "Component:UI UnlitMaterial")** | The material to use for an overlay effect. |
| `_topBorderMaterial` | **[UV\_RectMaterial](https://wiki.resonite.com/Component:UV_RectMaterial "Component:UV RectMaterial")** | The material to use for the top border. |
| `_screenBorderMaterial` | **[UV\_RectMaterial](https://wiki.resonite.com/Component:UV_RectMaterial "Component:UV RectMaterial")** | The material to use for the screen border. |
| `_buttonsBorderMaterial` | **[UV\_RectMaterial](https://wiki.resonite.com/Component:UV_RectMaterial "Component:UV RectMaterial")** | The material to use for the buttons border. |
| `_renderRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to render with the camera to create the visual for the curved screen. |
| `_topRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the top element renderable. |
| `_screenRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the screen element renderable. |
| `_buttonsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the button element renderable. |
| `_visualsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the visuals. |
| `_effectRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of special effects. |
| `_topCanvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The UIX canvas of the top element. |
| `_buttonsUIroot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the buttons element. |
| `_buttonsCanvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The UIX canvas of the buttons element. |
| `_style` | **[ParticleStyle](https://wiki.resonite.com/Component:ParticleStyle "Component:ParticleStyle")** | The style of the particle system creating the screen animation opening and closing edge. |
| `_particleColors` | **[ColorRangeInitializer](https://wiki.resonite.com/Component:ColorRangeInitializer "Component:ColorRangeInitializer")** | The color of the particles being spawned in when the dash is opening and closing. |
| `_emitter` | **[MeshEmitter](https://wiki.resonite.com/Component:MeshEmitter "Component:MeshEmitter")** | The emitter for the opening and closing animation. |
| `_topCollider` | **[MeshCollider](https://wiki.resonite.com/Component:MeshCollider "Component:MeshCollider")** | The collider for the top element. |
| `_screenCollider` | **[MeshCollider](https://wiki.resonite.com/Component:MeshCollider "Component:MeshCollider")** | The collider for the screens element. |
| `_buttonsCollider` | **[MeshCollider](https://wiki.resonite.com/Component:MeshCollider "Component:MeshCollider")** | The collider for the buttons element. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``IsRenderRoot:Func`3<ICollider, Int, Bool>`` | **[Func\`3](https://wiki.resonite.com/Type:Func%603 "Type:Func`3") < [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"), [Int](https://wiki.resonite.com/Type:Int "Type:Int"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | ✓ | Can be used to filter a raycast portal to only hit items that are part of the colliders under this component's render root. |

Triggers
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RadiantDash&oldid=113234](https://wiki.resonite.com/index.php?title=Component:RadiantDash&oldid=113234)"

Contents