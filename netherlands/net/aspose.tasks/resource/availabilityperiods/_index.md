---
title: "Resource.AvailabilityPeriods"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Resource-eigenschap. Haalt een instantie op van de AvailabilityPeriodCollection-klasse. De verzameling van perioden waarin een resource beschikbaar is."
type: docs
weight: 130
url: /nl/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

Haalt een instantie op van de [`AvailabilityPeriodCollection`](../../availabilityperiodcollection/) klasse. De verzameling van perioden waarin een resource beschikbaar is.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## Voorbeelden

Toont hoe een beschikbaarheidsperiode aan een resource kan worden toegevoegd.

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

### Zie ook

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


