# Component:ValueOptionDescriptionDriver

> Source: https://wiki.resonite.com/Component:ValueOptionDescriptionDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/72/ValueOptionDescriptionDriver%601Component.png/510px-ValueOptionDescriptionDriver%601Component.png)](https://wiki.resonite.com/File:ValueOptionDescriptionDriver%601Component.png) **Value Option Description Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ValueOptionDescriptionDriver** component is used primarily to [drive](https://wiki.resonite.com/Drive "Drive") the parts that make up a [Context Menu Item Source](https://wiki.resonite.com/Component:ContextMenuItemSource "Component:ContextMenuItemSource"). This component along with ContextMenuItemSource is used in [context menus](https://wiki.resonite.com/Context_menu "Context menu") for toggles where the toggle controls a [value](https://wiki.resonite.com/Value_Type "Value Type").

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Value` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>>** | The value field to compare against. |
| `ForceDeselected` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Forces any context menu item source to change regardless if it is deselected. |
| `Label` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string to set to the chosen label in the list of `Options`. |
| `Color` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to set to the chosen color in the list of `Options` |
| `Sprite` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") < [IAssetProvider\`1](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") < [Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite") >>** | The Sprite to set to the chosen Sprite in the list of `Options`. |
| `SpriteURL` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The sprite url. |
| `SpriteTint` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The sprite tint. |
| `DefaultOption` | _direct_ **[ValueOptionDescriptionDriver\`1.Option](https://wiki.resonite.com/Component:ValueOptionDescriptionDriver#Option) <T>** | The option to set `Label`, `Color`, and `Sprite` to when `Reference` doesn't match any `ReferenceTarget`s under the list of `Options`. |
| `Options` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ValueOptionDescriptionDriver\`1.Option](https://wiki.resonite.com/Component:ValueOptionDescriptionDriver#Option) <T>** | The list to search for a `ReferenceTarget` that matches `Value`. once a match is found, the option's `Label`, `Color`, and `Sprite` is used to drive this section's drive targets of `Label`, `Color`, and `Sprite`. |
| `SpriteTintBase` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Tints the entire sprite with a ColorX. |

Fields
Collapse

## Option

| Name | Type | Description |
| --- | --- | --- |
| `ReferenceValue` | [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") <T> | The values below should be used if `Value` is equal to this. |
| `Label` | [String](https://wiki.resonite.com/Type:String "Type:String") | The label to use if `ReferenceValue` matches `Value` |
| `Color` | [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") | The color to use if `ReferenceValue` matches `Value` |
| `Sprite` | [IAssetProvider\`1](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") < [Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite") > | The sprite to use if `ReferenceValue` matches `Value` |
| `SpriteTint` | [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") | The tint color for this sprite. |

Fields

## Usage

This component can be more efficient than using a bunch of [Value Equality Drivers](https://wiki.resonite.com/Component:ValueEqualityDriver "Component:ValueEqualityDriver") and generating a number based on such, or using [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") for a context menu.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ValueOptionDescriptionDriver&oldid=97819](https://wiki.resonite.com/index.php?title=Component:ValueOptionDescriptionDriver&oldid=97819)"

Contents