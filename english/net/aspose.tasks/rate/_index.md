---
title: Class Rate
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Rate class. Represents a definition of a time period and rates applicable for a resource during that period
type: docs
weight: 1550
url: /net/aspose.tasks/rate/
---
## Rate class

Represents a definition of a time period and rates applicable for a resource during that period.

```csharp
public class Rate
```

## Properties

| Name | Description |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | Gets or sets the cost per use of a resource. This value retrieved from the current date if a rate table exists for a resource. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | Gets or sets the overtime rate per hour for a resource. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Gets or sets the units used by Microsoft Project to display the overtime rate. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | Gets or sets the date when a rate becomes effective. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | Gets or sets the last date when a rate is effective. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | Gets or sets the unique identifier of a rate table for a resource. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | Gets or sets the standard rate per hour for a resource. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Gets or sets the units used by Microsoft Project to display the standard rate. |

## Examples

Shows how to work with resource rates.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RateTable = RateType.A;
rate1.RatesFrom = new DateTime(2019, 1, 1, 8, 0, 0);
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;
rate1.OvertimeRate = 10m;
rate1.OvertimeRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0));
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;
rate2.CostPerUse = 2m;

// work with the project...
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


