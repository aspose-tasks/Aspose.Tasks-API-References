---
title: "Resource.AvailabilityPeriods"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Resource. Obtient une instance de la classe AvailabilityPeriodCollection. La collection des périodes pendant lesquelles une ressource est disponible"
type: docs
weight: 130
url: /fr/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

Obtient une instance de la classe [`AvailabilityPeriodCollection`](../../availabilityperiodcollection/). La collection des périodes pendant lesquelles une ressource est disponible.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## Exemples

Montre comment ajouter une période de disponibilité pour une ressource.

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

### Voir aussi

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


