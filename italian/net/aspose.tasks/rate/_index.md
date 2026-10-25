---
title: "Classe Rate"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Rate. Rappresenta una definizione di un periodo di tempo e le tariffe applicabili a una risorsa durante quel periodo"
type: docs
weight: 1610
url: /it/net/aspose.tasks/rate/
---
## Rate class

Rappresenta una definizione di un periodo di tempo e delle tariffe applicabili a una risorsa durante tale periodo.

```csharp
public class Rate
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | Ottiene o imposta il costo per utilizzo di una risorsa. Questo valore viene recuperato dalla data corrente se esiste una tabella delle tariffe per una risorsa. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | Ottiene o imposta la tariffa di straordinario per ora per una risorsa. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Ottiene o imposta le unità utilizzate da Microsoft Project per visualizzare la tariffa di straordinario. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | Ottiene o imposta la data in cui una tariffa diventa efficace. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | Ottiene o imposta l'ultima data in cui una tariffa è efficace. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | Ottiene o imposta l'identificatore univoco di una tabella delle tariffe per una risorsa. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | Ottiene o imposta la tariffa standard per ora per una risorsa. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Ottiene o imposta le unità utilizzate da Microsoft Project per visualizzare la tariffa standard. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


