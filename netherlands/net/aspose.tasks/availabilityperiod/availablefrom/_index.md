---
title: "AvailabilityPeriod.AvailableFrom"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "AvailabilityPeriod-eigenschap. Haalt de datum op waarop een resource beschikbaar wordt voor de opgegeven periode of stelt deze in"
type: docs
weight: 20
url: /nl/net/aspose.tasks/availabilityperiod/availablefrom/
---
## AvailabilityPeriod.AvailableFrom property

Haalt op of stelt de datum in waarop een resource beschikbaar wordt voor de opgegeven periode.

```csharp
public DateTime AvailableFrom { get; set; }
```

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

* class [AvailabilityPeriod](../)
* namespace [Aspose.Tasks](../../availabilityperiod/)
* assembly [Aspose.Tasks](../../../)


