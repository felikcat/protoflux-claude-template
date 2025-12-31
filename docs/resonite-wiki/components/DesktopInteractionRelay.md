# Component:DesktopInteractionRelay

> Source: https://wiki.resonite.com/Component:DesktopInteractionRelay

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a5/DesktopInteractionRelayComponent.png/510px-DesktopInteractionRelayComponent.png)](https://wiki.resonite.com/File:DesktopInteractionRelayComponent.png) **Desktop Interaction Relay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DesktopInteractionRelay** component only works in user space. When part of a UIX, it sends events from user inputs (the position is determined by the [RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")) to the desktop display at `DisplayIndex`

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DisplayIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The display to send Interactions to. |
| `UseLegacyTextInput` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the legacy text input system. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DesktopInteractionRelay&oldid=94519](https://wiki.resonite.com/index.php?title=Component:DesktopInteractionRelay&oldid=94519)"

Contents