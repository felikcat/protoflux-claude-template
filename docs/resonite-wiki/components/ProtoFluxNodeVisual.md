# Component:ProtoFluxNodeVisual

> Source: https://wiki.resonite.com/Component:ProtoFluxNodeVisual

Collapse **Component image**

[File:ProtoFluxNodeVisualComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFluxNodeVisualComponent.png "File:ProtoFluxNodeVisualComponent.png") **Proto Flux Node Visual** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ProtoFluxNodeVisual** component is used to manage the visuals and interaction with ProtoFlux nodes when they are unpacked.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Node` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [ProtoFluxNode](https://wiki.resonite.com/Type:ProtoFluxNode "Type:ProtoFluxNode") >** | The protoflux node this is a visual for. |
| `IsSelected` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not this node is selected. |
| `IsHighlighted` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not this node is highlighted. |
| `_nodeHoverArea` | **[HoverArea](https://wiki.resonite.com/Component:HoverArea "Component:HoverArea")** | The Hover interaction area for this visual. |
| `_bgImage` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The background image for tye protoflux visual. |
| `_inputsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the different slots for node inputs. |
| `_outputsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the different slots for node outputs. |
| `_referencesRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot for references to other nodes like arrows for protoflux variables/globals. |
| `_overviewVisual` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field for enabling the overview alt version of this node. |
| `_overviewBg` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The BG color of the overview version of the visual. |
| `_labelBg` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field of the label BG. |
| `_labelText` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The enabled field of the label text. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProtoFluxNodeVisual&oldid=106517](https://wiki.resonite.com/index.php?title=Component:ProtoFluxNodeVisual&oldid=106517)"

Contents