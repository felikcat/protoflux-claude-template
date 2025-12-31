# Component:PointerInteractionController

> Source: https://wiki.resonite.com/Component:PointerInteractionController

Collapse **Component image**

[File:PointerInteractionControllerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=PointerInteractionControllerComponent.png "File:PointerInteractionControllerComponent.png") **Pointer Interaction Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PointerInteractionController** component is used by the game internally to handle tip touch source behavior on a user.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``GetTipPosition:Func`2<RelayTouchSource, Float3>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource"), [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | ✓ | Can be called to get where the tip position of the pointer is given a [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource") component. |
| ``GetTipDirection:Func`2<RelayTouchSource, Float3>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource"), [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | ✓ | Can be called to get where the tip direction of the pointer is given a [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource") component. |
| ``GetTouchType:Func`2<RelayTouchSource, TouchType>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource"), [TouchType](https://wiki.resonite.com/Type:TouchType "Type:TouchType") >** | ✓ | Can be called to get where the touch type of the pointer is currently, given a [RelayTouchSource](https://wiki.resonite.com/Component:RelayTouchSource "Component:RelayTouchSource") component. |
| `GetTouchable:TouchableGetter` | **[TouchableGetter](https://wiki.resonite.com/index.php?title=Type:TouchableGetter&action=edit&redlink=1 "Type:TouchableGetter (page does not exist)")** | ✓ | Can be called to get the touchable target object of this component. |

Triggers
Collapse

## Usage

Not to be used by the user, is used in internal game behavior.

## Examples

Tip touch source system execution.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PointerInteractionController&oldid=99089](https://wiki.resonite.com/index.php?title=Component:PointerInteractionController&oldid=99089)"

Contents