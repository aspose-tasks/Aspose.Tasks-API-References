---
title: "Resource.AvailabilityPeriods"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Resource. Λαμβάνει το στιγμιότυπο της κλάσης AvailabilityPeriodCollection. Η συλλογή των περιόδων κατά τις οποίες ένας πόρος είναι διαθέσιμος"
type: docs
weight: 130
url: /el/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

Λαμβάνει το στιγμιότυπο της κλάσης [`AvailabilityPeriodCollection`](../../availabilityperiodcollection/). Η συλλογή των περιόδων κατά τις οποίες ένας πόρος είναι διαθέσιμος.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## Παραδείγματα

Δείχνει πώς να προσθέσετε περίοδο διαθεσιμότητας για έναν πόρο.

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

### Δείτε επίσης

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


