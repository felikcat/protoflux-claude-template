# Component:RadiantDashButton

> Source: https://wiki.resonite.com/Component:RadiantDashButton

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6a/RadiantDashButtonComponent.png/510px-RadiantDashButtonComponent.png)](https://wiki.resonite.com/File:RadiantDashButtonComponent.png) **Radiant Dash Button** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Dash menu](https://wiki.resonite.com/Dash_menu "Dash menu").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Dash` | **[RadiantDash](https://wiki.resonite.com/Component:RadiantDash "Component:RadiantDash")** | The dash this is a button to. |
| `Screen` | **[RadiantDashScreen](https://wiki.resonite.com/Component:RadiantDashScreen "Component:RadiantDashScreen")** | The screen this button triggers a switch to for. |
| `_switchingEnabled` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | The field to drive with whether switching is enabled. |
| `_screenEnabled` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | The field to drive with whether the screen is enabled. |
| `_currentScreen` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [RadiantDashScreen](https://wiki.resonite.com/Component:RadiantDashScreen "Component:RadiantDashScreen") >>** | The current screen `Dash` is on. |
| `_button` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to trigger switching to the target screen. |
| `_text` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text for the button. |
| `_textBg` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The text background element. |
| `_icon` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The icon for the button. |
| `_layout` | **[LayoutElement](https://wiki.resonite.com/Component:LayoutElement "Component:LayoutElement")** | The layout UIX element of the button. |
| `_rootRect` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The root Rect UIX element for this button. |
| `_iconRect` | **[RectTransform](https://wiki.resonite.com/Component:RectTransform "Component:RectTransform")** | The root Rect UIX element for the button's icon. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RadiantDashButton&oldid=106532](https://wiki.resonite.com/index.php?title=Component:RadiantDashButton&oldid=106532)"

Contents