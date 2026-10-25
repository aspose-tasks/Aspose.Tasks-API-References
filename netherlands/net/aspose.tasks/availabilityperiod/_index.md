---
title: "Class AvailabilityPeriod"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.AvailabilityPeriod class. Vertegenwoordigt een periode waarin een resource beschikbaar is"
type: docs
weight: 80
url: /nl/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

Stelt een periode voor waarin een resource beschikbaar is.

```csharp
public class AvailabilityPeriod
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | Initialiseert een nieuw exemplaar van de `AvailabilityPeriod`. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | Initialiseert een nieuw exemplaar van de `AvailabilityPeriod` met het opgegeven datumbereik en beschikbare eenheden. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | Haalt op of stelt de datum in waarop een resource beschikbaar wordt voor de opgegeven periode. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | Haalt op of stelt de laatste datum in waarop een resource beschikbaar is voor de opgegeven periode. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | Haalt op of stelt het percentage van een resource in dat beschikbaar is gedurende de opgegeven periode. |

## Voorbeelden

Toont hoe beschikbaarheidsperioden voor een resource te maken.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // Voeg beschikbaarheidsperioden toe aan nieuwe resource
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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


