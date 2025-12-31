# Component:CloudStorageSpaceIndicator

> Source: https://wiki.resonite.com/Component:CloudStorageSpaceIndicator

(Redirected from [Component:CloudStorageSpaceIndicator](https://wiki.resonite.com/index.php?title=Component:CloudStorageSpaceIndicator&redirect=no "Component:CloudStorageSpaceIndicator"))

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LegacyCloudStorageSpaceIndicator&diff=99013) which are not marked for translation.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/78/LegacyCloudStorageSpaceIndicatorComponent.png/510px-LegacyCloudStorageSpaceIndicatorComponent.png)](https://wiki.resonite.com/File:LegacyCloudStorageSpaceIndicatorComponent.png) **Legacy Cloud Storage Space Indicator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyCloudStorageSpaceIndicator** component was used in old migrated legacy content that showed the cloud storage usage for a user. This component should not be used in new content and should be replaced when possible.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[StorageUsageStatus](https://wiki.resonite.com/Component:StorageUsageStatus "Component:StorageUsageStatus")** | The source of the cloud usage data. |
| `ContainerColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the UI container. |
| `UsedColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The normal color when storage has been used. |
| `LowSpaceColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use when space is low. |
| `CriticalSpaceColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color to use when space is almost filled or beyond filled. |
| `LowSpaceThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The percentage 0 to 1 for cloud storage to be considered low space. |
| `CriticalSpaceThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The percentage from 0 to 1 for cloud storage to be considered critically full. |
| `_ownerLabel` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer that shows the owner of this cloud storage indicator. |
| `_usageLabel` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer that shows the usage of the cloud storage for the user. |
| `_percentLabel` | **[TextRenderer](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer")** | The text renderer that shows the percentage full for the cloud storage of the user. |
| `_progressBar` | **[LegacyProgressBar](https://wiki.resonite.com/Component:LegacyProgressBar "Component:LegacyProgressBar")** | The UI used to show the amount of storage used as a progress bar. |
| `__legacyOwnerId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The legacy owner ID for what user this component was supposed to show the cloud storage for. |
| `__legacyMemberQuota` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component was supposed to show the amount of storage a user was using for a group shared storage that they were allocated. |

Fields
Collapse

## Usage

Just don't.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyCloudStorageSpaceIndicator&oldid=99013](https://wiki.resonite.com/index.php?title=Component:LegacyCloudStorageSpaceIndicator&oldid=99013)"

Contents