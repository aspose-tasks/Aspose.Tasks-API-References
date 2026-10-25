---
title: "AvailabilityPeriod.AvailableFrom"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété AvailabilityPeriod. Obtient ou définit la date à laquelle une ressource devient disponible pour la période spécifiée"
type: docs
weight: 20
url: /fr/net/aspose.tasks/availabilityperiod/availablefrom/
---
## AvailabilityPeriod.AvailableFrom property

Obtient ou définit la date à laquelle une ressource devient disponible pour la période spécifiée.

```csharp
public DateTime AvailableFrom { get; set; }
```

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

* class [AvailabilityPeriod](../)
* namespace [Aspose.Tasks](../../availabilityperiod/)
* assembly [Aspose.Tasks](../../../)


