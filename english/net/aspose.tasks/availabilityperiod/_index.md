---
title: Class AvailabilityPeriod
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.AvailabilityPeriod class. Represents a period when a resource is available
type: docs
weight: 80
url: /net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

Represents a period when a resource is available.

```csharp
public class AvailabilityPeriod
```

## Constructors

| Name | Description |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | Initializes a new instance of the `AvailabilityPeriod`. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | Initializes a new instance of the `AvailabilityPeriod` with the specified date range and available units. |

## Properties

| Name | Description |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | Gets or sets the date when a resource becomes available for the specified period. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | Gets or sets the last date when a resource is available for the specified period. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | Gets or sets the percentage of a resource which is available during the specified period. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


