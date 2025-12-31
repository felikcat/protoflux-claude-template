# ProtoFlux:UserNetworkStatistic

> Source: https://wiki.resonite.com/ProtoFlux:UserNetworkStatistic

User Network Statistic<T>

Name

\*

User

Info

The `User Network Statistic` node can output different statistics pertaining to a user's network connection in Resonite.

## Inputs

### Name ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The name of the network statistic the user would like to output. The output will only work if you select the correct type when slecting the node. There are different names depending on whether the user has connected through LNL or Steam Networking Sockets.

#### Any Connection Names

(These names apply to any type of network connection)

| Name | Type | Description |
| --- | --- | --- |
| `Protocol` | string | Outputs either "LNL" or "Steam", depending on the user's connection. |

#### LNL Connection Names

(These names only apply if the user is connected through LNL)

| Name | Type | Description |
| --- | --- | --- |
| `PrimaryChannelQueue` | int |  |
| `BackgroundChannelQueue` | int |  |
| `PacketsLost` | long |  |
| `PacketsSent` | long |  |
| `PacketsReceived` | long |  |
| `BytesSent` | long |  |
| `BytesReceived` | long |  |
| `WindowWaitCount` | long |  |
| `AveragePacketSize` | double |  |
| `AverageMergedPackets` | double |  |
| `MTU` | int |  |
| `TimeSinceLastPacket` | int |  |
| `RelayName` | string |  |

#### Steam Connection Names

(These names only apply if the user is connected through Steam Networking Sockets)

| Name | Type | Description |
| --- | --- | --- |
| `MainQualityLocal` | float |  |
| `MainQualityRemote` | float |  |
| `MainPendingReliable` | int |  |
| `MainPendingUnreliable` | int |  |
| `MainOutRate` | float |  |
| `MainInRate` | float |  |
| `BG_QualityLocal` | float |  |
| `BG_QualityRemote` | float |  |
| `BG_PendingReliable` | int |  |
| `BG_PendingUnreliable` | int |  |
| `BG_OutRate` | float |  |
| `BG_InRate` | float |  |
| `Bandwidth` | int |  |

### User ( [User](https://wiki.resonite.com/User "User"))

The user to show network statistics for. Does not work if user is host of the session.

## Outputs

This node will output a nullable value of the type specified for the associated statistic name. The ouput will always be null if user is the host of the session.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:UserNetworkStatistic&oldid=110985](https://wiki.resonite.com/index.php?title=ProtoFlux:UserNetworkStatistic&oldid=110985)"

Contents