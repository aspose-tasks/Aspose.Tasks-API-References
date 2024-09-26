---
title: Rate.CostPerUse
second_title: Aspose.Tasks for .NET API Reference
description: Rate property. Gets or sets the cost per use of a resource. This value retrieved from the current date if a rate table exists for a resource
type: docs
weight: 10
url: /net/aspose.tasks/rate/costperuse/
---
## Rate.CostPerUse property

Gets or sets the cost per use of a resource. This value retrieved from the current date if a rate table exists for a resource.

```csharp
public decimal CostPerUse { get; set; }
```

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

* class [Rate](../)
* namespace [Aspose.Tasks](../../rate/)
* assembly [Aspose.Tasks](../../../)


