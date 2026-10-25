---
title: "Rate.RatesTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Rate. Ottiene o imposta l'ultima data in cui una tariffa è efficace"
type: docs
weight: 50
url: /it/net/aspose.tasks/rate/ratesto/
---
## Rate.RatesTo property

Ottiene o imposta l'ultima data in cui una tariffa è efficace.

```csharp
public DateTime RatesTo { get; set; }
```

## Esempi

Mostra come lavorare con le tariffe delle risorse.

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

// lavorare con il progetto...
```

### Vedi anche

* class [Rate](../)
* namespace [Aspose.Tasks](../../rate/)
* assembly [Aspose.Tasks](../../../)


