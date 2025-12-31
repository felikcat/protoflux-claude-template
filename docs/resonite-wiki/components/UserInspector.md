# Component:UserInspector

> Source: https://wiki.resonite.com/Component:UserInspector

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e2/UserInspectorComponent.png/510px-UserInspectorComponent.png)](https://wiki.resonite.com/File:UserInspectorComponent.png) **User Inspector** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **User Inspector** component is better described on it's page, [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ViewUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user this inspector is currently updating through. |
| `ViewGroup` | **[UserInspector.View](https://wiki.resonite.com/Component:UserInspector#View)** | What kind of information group this is inspecting. |
| `ViewStreamGroup` | **[Ushort](https://wiki.resonite.com/Type:Ushort "Type:Ushort")** | The kind of value stream group this is viewing. |
| `_currentUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The current user this is viewing. |
| `_currentViewGroup` | **[UserInspector.View](https://wiki.resonite.com/Component:UserInspector#View)** | What kind of information group this is currently inspecting. |
| `_currentStreamGroup` | **[Ushort](https://wiki.resonite.com/Type:Ushort "Type:Ushort")** | The kind of value stream group this is currently viewing. |
| `_userListContentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to place user stream/properties content when viewing a user. |
| `_workersContentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to place user worker content when viewing a user. |
| `_userText` | **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The string field that stores text on the user being viewed. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``FilterWorker:Func`2<Worker, Bool>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | ✓ | A sync delegate that filters worker C# objects for the use of displaying those objects in this inspector. |

Triggers
Collapse

## Usage

See [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector").

## Examples

See [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector").

## See Also

- [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserInspector&oldid=100794](https://wiki.resonite.com/index.php?title=Component:UserInspector&oldid=100794)"

Contents