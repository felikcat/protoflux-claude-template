# Component:ContextMenuItem

> Source: https://wiki.resonite.com/Component:ContextMenuItem

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/68/ContextMenuItemComponent.png/510px-ContextMenuItemComponent.png)](https://wiki.resonite.com/File:ContextMenuItemComponent.png) **Context Menu Item** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A component that is used internally within [context menus](https://wiki.resonite.com/Context_menu "Context menu"). If you want to create a custom context menu, you should look at [ContextMenuItemSource](https://wiki.resonite.com/Component:ContextMenuItemSource "Component:ContextMenuItemSource").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Highlight` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Set and unset whether the item is being hovered over and should be highlighted. |
| `Icon` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The icon of this item. |
| `Sprite` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IAssetProvider\`1](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") < [Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite") >>** | The sprite of this item. |
| `Label` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The label element of this item. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of this item. |
| `_menu` | **[ContextMenu](https://wiki.resonite.com/Component:ContextMenu "Component:ContextMenu")** | This item's origin context menu. |
| `_highlighted` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The item is being hovered over. |
| `_arc` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The arc that makes up this item. |
| `_outerRadius` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field that specifies the outer radius of this item. |
| `_button` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that makes up this item. |

Fields
Collapse

## See Also

- [ContextMenuItemSource](https://wiki.resonite.com/Component:ContextMenuItemSource "Component:ContextMenuItemSource")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ContextMenuItem&oldid=98393](https://wiki.resonite.com/index.php?title=Component:ContextMenuItem&oldid=98393)"

Contents