---
title: AvailabilityPeriod.AvailableTo
second_title: Aspose.Tasks for .NET API Reference
description: AvailabilityPeriod property. Gets or sets the last date when a resource is available for the specified period
type: docs
weight: 30
url: /net/aspose.tasks/availabilityperiod/availableto/
---
## AvailabilityPeriod.AvailableTo property

Gets or sets the last date when a resource is available for the specified period.

```csharp
public DateTime AvailableTo { get; set; }
```

## Examples

Shows how to create availability periods for a resource.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // Add availability periods to new resource
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

### See Also

* class [AvailabilityPeriod](../)
* namespace [Aspose.Tasks](../../availabilityperiod/)
* assembly [Aspose.Tasks](../../../)


