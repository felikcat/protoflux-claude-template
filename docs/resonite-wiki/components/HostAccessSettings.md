# Component:HostAccessSettings

> Source: https://wiki.resonite.com/Component:HostAccessSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/df/HostAccessSettingsComponent.png/510px-HostAccessSettingsComponent.png)](https://wiki.resonite.com/File:HostAccessSettingsComponent.png) **Host Access Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Host Access Settings](https://wiki.resonite.com/Settings#Host_Access "Settings").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Entries` | _direct_ **[SyncDictionary\`2](https://wiki.resonite.com/index.php?title=Type:SyncDictionary%602&action=edit&redlink=1 "Type:SyncDictionary`2 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String"), [HostAccessSettings.Entry](https://wiki.resonite.com/Component:HostAccessSettings#Entry) >** | A list of allowed and denied IP address locations. |

Fields
Collapse

## Entry

| Name | Type | Description |
| --- | --- | --- |
| `AllowHTTP_Requests` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This indicayes of HTTP(S) requests are allowed for this host. These are typically REST API requests to communicate with third party services. |
| `AllowWebsockets` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This indicates if realtime Websocket connections are allowed for this host. These are often used for more realtime bi-directional communications and data streams. |
| `AllowOSC_Receiving` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This indicates if Resonite can receive and process OSC data |
| `AllowOSC_Sending` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This controls if Resonite is allowed to send data via OSC protocol to given host |
| `HTTP_RequestsSet` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `AllowHTTP_Requests` should be toggled soon. |
| `WebsocketsSet` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `AllowWebsockets` should be toggled soon. |
| `OSC_SenderSet` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `AllowOSC_Receiving` should be toggled soon. |
| `OSC_ReceiverSet` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `AllowOSC_Sending` should be toggled soon. |
| `LastHyperlinkRequestReason` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The last reason given for accessing a website. |
| `LastWebsocketRequestReason` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The last reason given for accessing a web socket. |
| `LastOSC_SenderRequestReason` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The last reason given for sending OSC data. |
| `LastOSC_ReceiverRequestReason` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The last reason given for receiving OSC data. |
| `AllowedPorts` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The number ports allowed from this entry address. |
| `BlockedPorts` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The number ports blocked from this entry address. |

Fields

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `GetEntry:SubsettingGetter` | **[SubsettingGetter](https://wiki.resonite.com/Type:SubsettingGetter "Type:SubsettingGetter")** | X | Gets an entry of type [HostAccessSettings.Entry](https://wiki.resonite.com/Component:HostAccessSettings#Entry) from the list of `Entries`. |

Triggers
Collapse

## Usage

See [Host Access Settings](https://wiki.resonite.com/Settings#Host_Access "Settings").

## Examples

See [Host Access Settings](https://wiki.resonite.com/Settings#Host_Access "Settings").

## See Also

- [Host Access Settings](https://wiki.resonite.com/Settings#Host_Access "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HostAccessSettings&oldid=99156](https://wiki.resonite.com/index.php?title=Component:HostAccessSettings&oldid=99156)"

Contents