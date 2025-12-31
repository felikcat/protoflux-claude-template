# Component:LocaleStringDriver

> Source: https://wiki.resonite.com/Component:LocaleStringDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/31/LocaleStringDriverComponent.png/510px-LocaleStringDriverComponent.png)](https://wiki.resonite.com/File:LocaleStringDriverComponent.png) **Locale String Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LocaleStringDriver** component is used to turn a key into a translated string from a locale, and then fill its value arguments with field contents or values.

## Usage

To use the LocaleStringDriver provide it with locale resource, a string to be driven and the name of the locale key you want to use. A list of all locale keys can be found in the [Yellow-Dog-Man/Locale repository](https://github.com/Yellow-Dog-Man/Locale/blob/main/en.json).

You can find a locale resource in the form of the [StaticLocaleProvider](https://wiki.resonite.com/Component:StaticLocaleProvider "Component:StaticLocaleProvider") component on the world Root slot.

If the locale string has no template arguments (for example "General.OK") this is all that you need to do. If it does have template parameters you will need to provide them using the ArgumentSources and ArgumentValues dictionaries. Because Resonite does not support editing Dictionaries through the scene inspector, you will need to use the [Sync Delegates](https://wiki.resonite.com/Component:LocaleStringDriver#Sync_Delegates) that the component exposes.

For example, if you want to format the "Dash.Exit.Header" key which in english has the value "Exit {appName}" you would need to provide the "appName" parameter using one of the dictionaries. The ArgumentValues dictionary will take priority over the ArgumentSources dictionary.

ArgumentSources maps parameter names to fields which will then be read to format the string. To add a parameter pull out the method proxy for SetArgumentSource and plug "appName" into Arg0 and a reference to the field you want to use. In this example you might want to use the PlatformName field of the PlatformInfo component.

ArgumentValues maps parameter names to values which will be directly used to format the string. To add a parameter pull out the method proxy for SetArgumentValue and plug "appName" into Arg0 and a string with the value you'd like into Arg1.

The Format field on the LocaleStringDriver component can also be used to add some extra text around the translated string, for example putting "Click here to {0}" would produce "Click here to Exit Resonite" with the above example.

[![](https://wiki.resonite.com/images/thumb/a/ac/LocaleStringDriverExample.jpg/600px-LocaleStringDriverExample.jpg)](https://wiki.resonite.com/File:LocaleStringDriverExample.jpg)

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string field to drive with the final locale translation. |
| `Key` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The locale key to get a translation with. |
| `Format` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | How to format the output. |
| `Locale` | **[LocaleResource](https://wiki.resonite.com/index.php?title=Type:LocaleResource&action=edit&redlink=1 "Type:LocaleResource (page does not exist)")** | The locale resource to use `Key` on to get the translated string for. |
| `ArgumentSources` | _direct_ **[SyncDictionary\`2](https://wiki.resonite.com/index.php?title=Type:SyncDictionary%602&action=edit&redlink=1 "Type:SyncDictionary`2 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String"), [RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [IField](https://wiki.resonite.com/Type:IField "Type:IField") >>** | A list of argument strings in a locale translation and their fields to get the values for them from. |
| `ArgumentValues` | _direct_ **[SyncDictionary\`2](https://wiki.resonite.com/index.php?title=Type:SyncDictionary%602&action=edit&redlink=1 "Type:SyncDictionary`2 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String"), [SyncVar](https://wiki.resonite.com/index.php?title=Type:SyncVar&action=edit&redlink=1 "Type:SyncVar (page does not exist)") >** | A list of argument strings in a locale translation and their values. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SetArgumentSource:Action`2<String, IField>`` | **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String"), [IField](https://wiki.resonite.com/Type:IField "Type:IField") >** | X | Can be called to set the argument source for the locale data. |
| ``SetArgumentValue:Func`3<String, Object, Bool>`` | **[Func\`3](https://wiki.resonite.com/Type:Func%603 "Type:Func`3") < [String](https://wiki.resonite.com/Type:String "Type:String"), [Object](https://wiki.resonite.com/Type:Object "Type:Object"), [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | X | Can be called to set the argument value for the locale data. |

Triggers
Collapse

\[\]

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocaleStringDriver&oldid=101204](https://wiki.resonite.com/index.php?title=Component:LocaleStringDriver&oldid=101204)"

Contents