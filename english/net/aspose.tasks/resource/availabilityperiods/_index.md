---
title: Resource.AvailabilityPeriods
second_title: Aspose.Tasks for .NET API Reference
description: Resource property. Gets a the instance of the AvailabilityPeriodCollection class. The collection of periods during which a resource is available
type: docs
weight: 130
url: /net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

Gets a the instance of the [`AvailabilityPeriodCollection`](../../availabilityperiodcollection/) class. The collection of periods during which a resource is available.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## Examples

Shows how to add availability period for a resource.

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

### See Also

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


