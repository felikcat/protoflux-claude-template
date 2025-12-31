# Component:FundingStatistics

> Source: https://wiki.resonite.com/Component:FundingStatistics

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/38/FundingStatisticsComponent.png/510px-FundingStatisticsComponent.png)](https://wiki.resonite.com/File:FundingStatisticsComponent.png) **Funding Statistics** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Funding Statistics** component is used to get the different funding values for Resonite in United States Dollars from supporters.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Timestamp` | **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | The last time the values were updated as a time stamp. |
| `Aggregate` | _direct_ **[FundingStatistics.ServiceStats](https://wiki.resonite.com/Component:FundingStatistics#ServiceStats)** | The combination of all support channels. |
| `Patreon` | _direct_ **[FundingStatistics.ServiceStats](https://wiki.resonite.com/Component:FundingStatistics#ServiceStats)** | The Monetary support from Patreon members. |
| `Stripe` | _direct_ **[FundingStatistics.ServiceStats](https://wiki.resonite.com/Component:FundingStatistics#ServiceStats)** | The Monetary support from Stripe members. |

Fields
Collapse

## ServiceStats

| Name | Type | Description |
| --- | --- | --- |
| `Current` | _direct_ **[FundingStatistics.FundingStats](https://wiki.resonite.com/Component:FundingStatistics#FundingStats)** | The current money being supported via this medium. |
| `Historical` | _direct_ **[FundingStatistics.FundingStats](https://wiki.resonite.com/Component:FundingStatistics#FundingStats)** | The historical money that was given via this medium. |

Fields

## FundingStats

| Name | Type | Description |
| --- | --- | --- |
| `TotalAmountUSD` | **[decimal](https://wiki.resonite.com/Type:Decimal "Type:Decimal")** | Total amount of money via this medium. |
| `AverageAmountUSD` | **[decimal](https://wiki.resonite.com/Type:Decimal "Type:Decimal")** | Average amount of money via this medium. |
| `TotalUniqueSupporters` | **[int](https://wiki.resonite.com/Type:Int "Type:Int")** | The total unique supporters that are supporting Resonite via this medium. |

Fields

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FundingStatistics&oldid=98408](https://wiki.resonite.com/index.php?title=Component:FundingStatistics&oldid=98408)"

Contents