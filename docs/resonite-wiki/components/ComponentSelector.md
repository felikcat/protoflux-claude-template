# Component:ComponentSelector

> Source: https://wiki.resonite.com/Component:ComponentSelector

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3d/ComponentSelectorComponent.png/510px-ComponentSelectorComponent.png)](https://wiki.resonite.com/File:ComponentSelectorComponent.png) **Component Selector** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Component Selector** is better understood on its page, [Complex Types in Components](https://wiki.resonite.com/Complex_Types_in_Components "Complex Types in Components").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ComponentSelected` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ComponentSelectionHandler](https://wiki.resonite.com/index.php?title=Type:ComponentSelectionHandler&action=edit&redlink=1 "Type:ComponentSelectionHandler (page does not exist)")** | The Sync delegate to call when the component is attached. |
| `ComponentFilter` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Predicate\`1](https://wiki.resonite.com/index.php?title=Type:Predicate%601&action=edit&redlink=1 "Type:Predicate`1 (page does not exist)") < [Type](https://wiki.resonite.com/Type:Type "Type:Type") >** | The type of Components to show in the attacher. |
| `GenericArgumentPrefiller` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[GenericArgumentPrefiller](https://wiki.resonite.com/index.php?title=Type:GenericArgumentPrefiller&action=edit&redlink=1 "Type:GenericArgumentPrefiller (page does not exist)")** | A sync delegate that fills the list of generic arguments for a selected type so it doesn't only ask for a certain type. |
| `_uiRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the UI. |
| `_rootPath` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The path that this is navigated to in the component attacher. |
| `_genericType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The generic type we are trying to make a generic fill for. |
| `_customGenericTypeLabel` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The label for the generic type we are attaching. |
| `_customGenericTypeColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color for the generic type we are attaching. |
| `_customGenericArguments` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The generic arguments being used for the current Component being attached. See [Complex Types in Components](https://wiki.resonite.com/Complex_Types_in_Components "Complex Types in Components"). |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnCancelPressed:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Closes the UI and doesn't attach anything. |
| ``OnOpenCategoryPressed:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | Opens a category of the path argument given. |
| ``OpenGenericTypesPressed:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | Handles loading the menu for selecting a generic argument screen for a component that has a generic argument like <T>, <A>, or ~~to name a few.~~ |
| ``OpenGroupPressed:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | Handles bringing up the menu for opening a group of components of the same type (purple buttons). |
| ``OnAddComponentPressed:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | Triggers when a component is addrd. |
| `OnCreateCustomType:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Triggers when a component is made via the attacher with a generic type that isn't in the list of preselected generics. |

Triggers
Collapse

## Usage

See [Complex Types in Components](https://wiki.resonite.com/Complex_Types_in_Components "Complex Types in Components").

## Examples

See [Complex Types in Components](https://wiki.resonite.com/Complex_Types_in_Components "Complex Types in Components").

## See Also

- [Complex Types in Components](https://wiki.resonite.com/Complex_Types_in_Components "Complex Types in Components")
- [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ComponentSelector&oldid=98352](https://wiki.resonite.com/index.php?title=Component:ComponentSelector&oldid=98352)"

Contents