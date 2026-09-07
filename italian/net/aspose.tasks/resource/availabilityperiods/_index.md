---
title: "Resource.AvailabilityPeriods"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Resource. Ottiene l'istanza della classe AvailabilityPeriodCollection. La raccolta di periodi durante i quali una risorsa è disponibile"
type: docs
weight: 130
url: /it/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

Ottiene l'istanza della classe [`AvailabilityPeriodCollection`](../../availabilityperiodcollection/). La raccolta di periodi durante i quali una risorsa è disponibile.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## Esempi

Mostra come aggiungere un periodo di disponibilità per una risorsa.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

var availabilityPeriod = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 1, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 1, 17, 0, 0),
    AvailableUnits = 2d
};
resource.AvailabilityPeriods.Add(availabilityPeriod);

var availabilityPeriod2 = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 2, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 2, 17, 0, 0),
    AvailableUnits = 3d
};
resource.AvailabilityPeriods.Add(availabilityPeriod2);
```

### Vedi anche

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


