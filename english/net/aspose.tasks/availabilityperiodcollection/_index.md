---
title: Class AvailabilityPeriodCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.AvailabilityPeriodCollection class. Represents a collection which contains AvailabilityPeriod objects
type: docs
weight: 90
url: /net/aspose.tasks/availabilityperiodcollection/
---
## AvailabilityPeriodCollection class

Represents a collection which contains [`AvailabilityPeriod`](../availabilityperiod/) objects.

```csharp
public class AvailabilityPeriodCollection : IList<AvailabilityPeriod>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/availabilityperiodcollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/availabilityperiodcollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |
| [Item](../../aspose.tasks/availabilityperiodcollection/item/) { get; set; } | Returns or sets the element at the specified index. |
| [ParentResource](../../aspose.tasks/availabilityperiodcollection/parentresource/) { get; } | Gets the parent [`Resource`](../resource/) for this object. Parent [`Resource`](../resource/) object for this collection. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/availabilityperiodcollection/add/)(AvailabilityPeriod) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/availabilityperiodcollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/availabilityperiodcollection/contains/)(AvailabilityPeriod) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/availabilityperiodcollection/copyto/)(AvailabilityPeriod[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/availabilityperiodcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [IndexOf](../../aspose.tasks/availabilityperiodcollection/indexof/)(AvailabilityPeriod) | Determines the index of the specified item in this collection. |
| [Insert](../../aspose.tasks/availabilityperiodcollection/insert/)(int, AvailabilityPeriod) | Inserts the specified item at the specified index. |
| [Remove](../../aspose.tasks/availabilityperiodcollection/remove/)(AvailabilityPeriod) | Removes the first occurrence of a specific object from this collection. |
| [RemoveAt](../../aspose.tasks/availabilityperiodcollection/removeat/)(int) | Removes an item at the specified index. |

## Examples

Shows how to work with availability period collection of resource.

```csharp
public void WorkWithAvailabilityPeriodCollection()
{
    var project = new Project(DataDir + "UpdateResourceData.mpp");
    var resource = project.Resources.GetById(1);

    resource.AvailabilityPeriods.Clear();

    // Add availability periods (2012 and 2014 years) to the new resource
    IEnumerable<AvailabilityPeriod> periods = this.GetPeriods();
    foreach (var period in periods)
    {
        if (!resource.AvailabilityPeriods.IsReadOnly)
        {
            resource.AvailabilityPeriods.Add(period);
        }
    }

    var period2013 = new AvailabilityPeriod { AvailableFrom = new DateTime(2013, 1, 1), AvailableTo = new DateTime(2013, 12, 12), AvailableUnits = 0.81 };

    if (!resource.AvailabilityPeriods.Contains(period2013))
    {
        resource.AvailabilityPeriods.Insert(1, period2013);
    }

    Console.WriteLine("Count of availability periods: " + resource.AvailabilityPeriods.Count);
    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }

    var periodsToCopy = new AvailabilityPeriod[resource.AvailabilityPeriods.Count];
    resource.AvailabilityPeriods.CopyTo(periodsToCopy, 0);

    var otherResource = project.Resources.GetById(2);
    otherResource.AvailabilityPeriods.Clear();
    foreach (var period in periodsToCopy)
    {
        otherResource.AvailabilityPeriods.Add(period);
    }

    var period2015 = new AvailabilityPeriod { AvailableFrom = new DateTime(2015, 1, 1), AvailableTo = new DateTime(2015, 12, 12), AvailableUnits = 0.50 };

    var period2016 = new AvailabilityPeriod { AvailableFrom = new DateTime(2016, 1, 1), AvailableTo = new DateTime(2016, 12, 12), AvailableUnits = 0.53 };

    if (otherResource.AvailabilityPeriods.IndexOf(period2015) < 0)
    {
        otherResource.AvailabilityPeriods.Add(period2015);
    }

    if (otherResource.AvailabilityPeriods.IndexOf(period2016) < 0)
    {
        otherResource.AvailabilityPeriods.Add(period2016);
    }

    // update available units for period of 2014 year
    otherResource.AvailabilityPeriods[otherResource.AvailabilityPeriods.Count - 2].AvailableUnits = 0.90;

    // remove period of 2013
    otherResource.AvailabilityPeriods.Remove(period2013);

    // remove period of 2011
    otherResource.AvailabilityPeriods.RemoveAt(0);

    Console.WriteLine("Print resource availability periods of the resource: " + otherResource.Get(Rsc.Name));
    Console.WriteLine("Count of availability periods: " + resource.AvailabilityPeriods.Count);
    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }
}

private IEnumerable<AvailabilityPeriod> GetPeriods()
{
    var periods = new List<AvailabilityPeriod>();
    var period = new AvailabilityPeriod { AvailableFrom = new DateTime(2012, 1, 1), AvailableTo = new DateTime(2012, 12, 12), AvailableUnits = 0.99 };
    periods.Add(period);

    var period2 = new AvailabilityPeriod { AvailableFrom = new DateTime(2014, 1, 1), AvailableTo = new DateTime(2014, 12, 12), AvailableUnits = 0.94 };
    periods.Add(period2);
    return periods;
}
```

### See Also

* class [AvailabilityPeriod](../availabilityperiod/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


