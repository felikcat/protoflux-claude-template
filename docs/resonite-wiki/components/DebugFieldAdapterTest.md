# Component:DebugFieldAdapterTest

> Source: https://wiki.resonite.com/Component:DebugFieldAdapterTest

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9d/DebugFieldAdapterTestComponent.png/510px-DebugFieldAdapterTestComponent.png)](https://wiki.resonite.com/File:DebugFieldAdapterTestComponent.png) **Debug Field Adapter Test** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugFieldAdapterTest** is used with [Component:DebugFieldAdapter](https://wiki.resonite.com/Component:DebugFieldAdapter "Component:DebugFieldAdapter") to test the accuracy. If set properly, the `InvertedColor` should flash between inverted and not inverted every frame.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `InvertedColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | `SourceColor` inverted. Doesn't do this when this component is by itself. Is set to `SourceColor` every time this component changes in any way. |
| `SourceColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The source color. Doesn't affect or is changed by anything. Except for sets or drives. |

Fields
Collapse

## Usage

Is a test item. Is not needed to be used by the user.

## See Also

- [Component:DebugFieldAdapter](https://wiki.resonite.com/Component:DebugFieldAdapter "Component:DebugFieldAdapter")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugFieldAdapterTest&oldid=96411](https://wiki.resonite.com/index.php?title=Component:DebugFieldAdapterTest&oldid=96411)"

Contents