---
title: "Rate.OvertimeRateFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rate-eigenschap. Haalt of stelt de eenheden in die door Microsoft Project worden gebruikt om het overurenttarief weer te geven."
type: docs
weight: 30
url: /nl/net/aspose.tasks/rate/overtimerateformat/
---
## Rate.OvertimeRateFormat property

Haalt op of stelt de eenheden in die Microsoft Project gebruikt om het overurenttarief weer te geven.

```csharp
public RateFormatType OvertimeRateFormat { get; set; }
```

## Voorbeelden

Toont hoe te werken met resource‑tarieven.

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

// werken met het project...
```

### Zie ook

* enum [RateFormatType](../../rateformattype/)
* class [Rate](../)
* namespace [Aspose.Tasks](../../rate/)
* assembly [Aspose.Tasks](../../../)


