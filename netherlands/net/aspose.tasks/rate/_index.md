---
title: "Klasse Rate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Rate‑klasse. Vertegenwoordigt een definitie van een tijdsperiode en tarieven die van toepassing zijn op een resource gedurende die periode"
type: docs
weight: 1610
url: /nl/net/aspose.tasks/rate/
---
## Rate class

Stelt een definitie voor van een tijdsperiode en tarieven die van toepassing zijn op een resource gedurende die periode.

```csharp
public class Rate
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | Haalt op of stelt de kosten per gebruik van een resource in. Deze waarde wordt opgehaald op basis van de huidige datum als er een tarieftabel voor een resource bestaat. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | Haalt op of stelt het overurenttarief per uur voor een resource in. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Haalt op of stelt de eenheden in die Microsoft Project gebruikt om het overurenttarief weer te geven. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | Haalt op of stelt de datum in waarop een tarief van kracht wordt. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | Haalt op of stelt de laatste datum in waarop een tarief van kracht is. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | Haalt op of stelt de unieke identifier van een tarieftabel voor een resource in. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | Haalt op of stelt het standaardtarief per uur voor een resource in. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Haalt op of stelt de eenheden in die Microsoft Project gebruikt om het standaardtarief weer te geven. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


