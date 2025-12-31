# Component:TouchableTextField

> Source: https://wiki.resonite.com/Component:TouchableTextField

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TouchableTextField&diff=94812) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/62/TouchableTextFieldComponent.png/510px-TouchableTextFieldComponent.png)](https://wiki.resonite.com/File:TouchableTextFieldComponent.png) **Touchable Text Field** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TouchableTextField** component, similar to a [TextField](https://wiki.resonite.com/Component:TextField "Component:TextField") for [UIX](https://wiki.resonite.com/UIX "UIX"), this component when combined with a [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") on the same [slot](https://wiki.resonite.com/Slot "Slot"), will allow any text in the [world](https://wiki.resonite.com/World "World") to be clicked on to make it become editable.

This allows the text to be edited in both directions: In the component and in the world directly.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TextEditor` | **[TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor")** | The [TextField](https://wiki.resonite.com/Component:TextField "Component:TextField") to allow for bi-directional editing. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow interaction with this component if it is out of the user's view. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allows for the user to only edit this text in [Edit Mode](https://wiki.resonite.com/Edit_Mode "Edit Mode"). |
| `ActiveUserRootOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allows to only be editable when under the active user. |

Fields
Collapse

## Usage

Great for when you don't want to be bound by [UIX](https://wiki.resonite.com/UIX "UIX") to make editable texts.

If the text is not responding or is not editing properly, try adding the [BoxCollider](https://wiki.resonite.com/Component:BoxCollider "Component:BoxCollider") component.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TouchableTextField&oldid=94812](https://wiki.resonite.com/index.php?title=Component:TouchableTextField&oldid=94812)"

Contents