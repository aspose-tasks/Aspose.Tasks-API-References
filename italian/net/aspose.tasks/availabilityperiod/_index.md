---
title: "Classe AvailabilityPeriod"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.AvailabilityPeriod. Rappresenta un periodo in cui una risorsa è disponibile"
type: docs
weight: 80
url: /it/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

Rappresenta un periodo in cui una risorsa è disponibile.

```csharp
public class AvailabilityPeriod
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | Inizializza una nuova istanza di `AvailabilityPeriod`. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | Inizializza una nuova istanza di `AvailabilityPeriod` con l'intervallo di date specificato e le unità disponibili. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | Ottiene o imposta la data in cui una risorsa diventa disponibile per il periodo specificato. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | Ottiene o imposta l'ultima data in cui una risorsa è disponibile per il periodo specificato. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | Ottiene o imposta la percentuale di una risorsa disponibile durante il periodo specificato. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


