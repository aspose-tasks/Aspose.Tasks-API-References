---
title: "AvailabilityPeriod.AvailableUnits"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà AvailabilityPeriod. Ottiene o imposta la percentuale di una risorsa disponibile durante il periodo specificato"
type: docs
weight: 40
url: /it/net/aspose.tasks/availabilityperiod/availableunits/
---
## AvailabilityPeriod.AvailableUnits property

Ottiene o imposta la percentuale di una risorsa disponibile durante il periodo specificato.

```csharp
public double AvailableUnits { get; set; }
```

## Esempi

Mostra come creare periodi di disponibilità per una risorsa.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // Aggiungi periodi di disponibilità alla nuova risorsa
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

### Vedi anche

* class [AvailabilityPeriod](../)
* namespace [Aspose.Tasks](../../availabilityperiod/)
* assembly [Aspose.Tasks](../../../)


