# Component:ParticleSpray

> Source: https://wiki.resonite.com/Component:ParticleSpray

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f9/ParticleSprayComponent.png/510px-ParticleSprayComponent.png)](https://wiki.resonite.com/File:ParticleSprayComponent.png) **Particle Spray** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ParticleSpray** component is a tool that shoots particles when the trigger is pulled.

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
| `Rate` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Ths rate at which the spray tip sprays at max (primary strength is raised to `RateExp` first before multiplying with this) |
| `RateExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | primary strength of the tool is raised to this number. |
| `MinSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The min speed the particles travel at. |
| `MaxSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The max speed the particles travel at. |
| `partStyle` | **[ParticleStyle](https://wiki.resonite.com/Component:ParticleStyle "Component:ParticleStyle")** | The style of the particles. |
| `partSpeed` | **[SpeedRangeInitializer](https://wiki.resonite.com/Component:SpeedRangeInitializer "Component:SpeedRangeInitializer")** | The min/max speed the particles travel at, is synced with `MinSpeed` and `MaxSpeed` |
| `partEmitter` | **[ParticleEmitter](https://wiki.resonite.com/index.php?title=Type:ParticleEmitter&action=edit&redlink=1 "Type:ParticleEmitter (page does not exist)")** | the Particle emitter this particle spray is controlling. |

Fields
Collapse

## See Also

- [ITool](https://wiki.resonite.com/Type:ITool "Type:ITool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ParticleSpray&oldid=98785](https://wiki.resonite.com/index.php?title=Component:ParticleSpray&oldid=98785)"

Contents