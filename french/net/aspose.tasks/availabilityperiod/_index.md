---
title: "Classe AvailabilityPeriod"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.AvailabilityPeriod class. Représente une période pendant laquelle une ressource est disponible"
type: docs
weight: 80
url: /fr/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

Représente une période pendant laquelle une ressource est disponible.

```csharp
public class AvailabilityPeriod
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | Initialise une nouvelle instance de `AvailabilityPeriod`. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | Initialise une nouvelle instance de `AvailabilityPeriod` avec la plage de dates spécifiée et les unités disponibles. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | Obtient ou définit la date à laquelle une ressource devient disponible pour la période spécifiée. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | Obtient ou définit la dernière date à laquelle une ressource est disponible pour la période spécifiée. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | Obtient ou définit le pourcentage d'une ressource qui est disponible pendant la période spécifiée. |

## Exemples

Montre comment créer des périodes de disponibilité pour une ressource.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // Ajouter des périodes de disponibilité à une nouvelle ressource
    IEnumerable<AvailabilityPeriod> periods = GetPeriods();
    foreach (var period in periods)
    {
        resource.AvailabilityPeriods.Add(period);
    }

    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }
}

private static IEnumerable<AvailabilityPeriod> GetPeriods()
{
    var periods = new List<AvailabilityPeriod>(2);
    var period = new AvailabilityPeriod
    {
        AvailableFrom = new DateTime(2011, 12, 12),
        AvailableTo = new DateTime(2013, 12, 12),
        AvailableUnits = 0.99
    };

    periods.Add(period);

    var period2 = new AvailabilityPeriod
    {
        AvailableFrom = new DateTime(2013, 12, 12),
        AvailableTo = new DateTime(2015, 12, 12),
        AvailableUnits = 0.94
    };
    periods.Add(period2);
    return periods;
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


