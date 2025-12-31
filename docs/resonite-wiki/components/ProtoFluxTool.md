# Component:ProtoFluxTool

> Source: https://wiki.resonite.com/Component:ProtoFluxTool

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3f/ProtoFluxToolComponent.png/510px-ProtoFluxToolComponent.png)](https://wiki.resonite.com/File:ProtoFluxToolComponent.png) **Proto Flux Tool** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

For more info on the protoflux tool in general, see [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") and [ProtoFlux Tool](https://wiki.resonite.com/ProtoFlux_Tool "ProtoFlux Tool").

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
| `SpawnNodeType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The type of the ProtoFlux node to spawn. |
| `WirePoint` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that the tool is currently pulling a wire out of. |
| `MaxConnectDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance this protoflux tool will search for nodes from it's tip before stopping. it's usually 20 meters in local space. |
| `SelectionProgress` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far the user is to selecting nodes by holding [Secondary](https://wiki.resonite.com/Controls "Controls") |
| `HoveringElementName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the protoflux element this tool is currently hovering over |
| `HoveringElementContentType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The type of the protoflux element this tool is currently hovering over |
| `HoveringElementColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of `HoveringElementContentType` |
| `_selectedNodes` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[ProtoFluxNodeVisual](https://wiki.resonite.com/Component:ProtoFluxNodeVisual "Component:ProtoFluxNodeVisual")** | The list of nodes the protoflux nodes that the tool currently has selected. |
| `_wirePointPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | What field to drive on a [StripeMesh](https://wiki.resonite.com/Component:StripeMesh "Component:StripeMesh") for a currently pulled wire. |
| `_text` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text to drive with information from this tool. |
| `_currentProxy` | **[ProtoFluxElementProxy](https://wiki.resonite.com/index.php?title=Type:ProtoFluxElementProxy&action=edit&redlink=1 "Type:ProtoFluxElementProxy (page does not exist)")** | What element the protoflux tool is currently pulling in order to connect to another element via the UI. |
| `_currentTempWire` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The current wire that this tool is pulling from a protoflux connector. |
| `_currentCutLine` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The current wire that this tool is trying to cut. |
| `_cutLineScale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The current wire that this tool is trying to cut's scale. |
| `_cutLineOrientation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The orientation of the current wire that this tool is trying to cut. |
| `_currentHighlightedNode` | **[ProtoFluxNodeVisual](https://wiki.resonite.com/Component:ProtoFluxNodeVisual "Component:ProtoFluxNodeVisual")** | The current node this tool is looking at. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `ToggleOverviewMode:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the toggle overview mode button is touched. |
| ``OnPackInPlace:ButtonEventHandler`1<ProtoFluxNode>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [ProtoFluxNode](https://wiki.resonite.com/Type:ProtoFluxNode "Type:ProtoFluxNode") >** | ✓ | Called when the pack in place button is touched. |
| ``OnUnpack:ButtonEventHandler`1<Slot>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | ✓ | Called when the unpack button is touched. |
| `OnClearSelection:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the clear selection button is touched. |
| `OpenNodeBrowser:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the open node browser button is touched. |
| ``OnCreateDrive:ButtonEventHandler`1<IWorldElement>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [IWorldElement](https://wiki.resonite.com/Type:IWorldElement "Type:IWorldElement") >** | ✓ | Called when the create drive button is touched. |
| ``OnCreateWrite:ButtonEventHandler`1<IWorldElement>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [IWorldElement](https://wiki.resonite.com/Type:IWorldElement "Type:IWorldElement") >** | ✓ | Called when the create write button is touched. |
| ``OnCreateLocal:ButtonEventHandler`1<ProtoFluxReferenceProxy>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [ProtoFluxReferenceProxy](https://wiki.resonite.com/Component:ProtoFluxReferenceProxy "Component:ProtoFluxReferenceProxy") >** | ✓ | Called when the create local button is touched. |
| ``OnCreateStore:ButtonEventHandler`1<ProtoFluxReferenceProxy>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [ProtoFluxReferenceProxy](https://wiki.resonite.com/Component:ProtoFluxReferenceProxy "Component:ProtoFluxReferenceProxy") >** | ✓ | Called when the create store button is touched. |
| ``OnCreateDataModelStore:ButtonEventHandler`1<ProtoFluxReferenceProxy>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [ProtoFluxReferenceProxy](https://wiki.resonite.com/Component:ProtoFluxReferenceProxy "Component:ProtoFluxReferenceProxy") >** | ✓ | Called when the create data model store button is touched. |
| ``OnCreateSource:ButtonEventHandler`1<IWorldElement>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [IWorldElement](https://wiki.resonite.com/Type:IWorldElement "Type:IWorldElement") >** | ✓ | Called when the create source button is touched. |
| ``OnCreateReference:ButtonEventHandler`1<IWorldElement>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [IWorldElement](https://wiki.resonite.com/Type:IWorldElement "Type:IWorldElement") >** | ✓ | Called when the create reference button is touched. |
| ``OnCreateDelegateProxy:ButtonEventHandler`1<Delegate>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Delegate](https://wiki.resonite.com/Type:Delegate "Type:Delegate") >** | ✓ | Called when the create delegate proxy button is touched. |

Triggers
Collapse

## Usage

## Examples

## See Also

- [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux")
- [ProtoFlux Tool](https://wiki.resonite.com/ProtoFlux_Tool "ProtoFlux Tool")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxTool&oldid=99106](https://wiki.resonite.com/index.php?title=Component:ProtoFluxTool&oldid=99106)"

Contents