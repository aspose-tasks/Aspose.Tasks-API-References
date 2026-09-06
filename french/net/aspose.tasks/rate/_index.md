---
title: "Classe Rate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Rate. Représente une définition d’une période de temps et les tarifs applicables à une ressource pendant cette période"
type: docs
weight: 1610
url: /fr/net/aspose.tasks/rate/
---
## Rate class

Représente une définition d'une période de temps et des tarifs applicables à une ressource pendant cette période.

```csharp
public class Rate
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CostPerUse](../../aspose.tasks/rate/costperuse/) { get; set; } | Obtient ou définit le coût par utilisation d’une ressource. Cette valeur est récupérée à la date actuelle si un tableau de tarifs existe pour une ressource. |
| [OvertimeRate](../../aspose.tasks/rate/overtimerate/) { get; set; } | Obtient ou définit le taux d’heures supplémentaires par heure pour une ressource. |
| [OvertimeRateFormat](../../aspose.tasks/rate/overtimerateformat/) { get; set; } | Obtient ou définit les unités utilisées par Microsoft Project pour afficher le taux d’heures supplémentaires. |
| [RatesFrom](../../aspose.tasks/rate/ratesfrom/) { get; set; } | Obtient ou définit la date à laquelle un tarif devient effectif. |
| [RatesTo](../../aspose.tasks/rate/ratesto/) { get; set; } | Obtient ou définit la dernière date à laquelle un tarif est effectif. |
| [RateTable](../../aspose.tasks/rate/ratetable/) { get; set; } | Obtient ou définit l’identifiant unique d’un tableau de tarifs pour une ressource. |
| [StandardRate](../../aspose.tasks/rate/standardrate/) { get; set; } | Obtient ou définit le tarif standard par heure pour une ressource. |
| [StandardRateFormat](../../aspose.tasks/rate/standardrateformat/) { get; set; } | Obtient ou définit les unités utilisées par Microsoft Project pour afficher le tarif standard. |

## Exemples

Montre comment travailler avec les tarifs des ressources.

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

// travailler avec le projet...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


