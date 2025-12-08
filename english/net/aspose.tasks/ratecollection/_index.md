---
title: Class RateCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RateCollection class. Represents a collection which contains Rate objects
type: docs
weight: 1600
url: /net/aspose.tasks/ratecollection/
---
## RateCollection class

Represents a collection which contains [`Rate`](../rate/) objects.

```csharp
public class RateCollection : IDictionary<RateType, RateByDateCollection>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/ratecollection/count/) { get; } | Gets the number of elements contained in the RateCollection. |
| [IsReadOnly](../../aspose.tasks/ratecollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read only. |
| [Item](../../aspose.tasks/ratecollection/item/) { get; set; } | Returns or sets the element at the specified index. |
| [ParentResource](../../aspose.tasks/ratecollection/parentresource/) { get; } | Gets the parent [`Resource`](../resource/) object for this collection. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/ratecollection/add/#add)(DateTime) | Adds a new [`Rate`](../rate/) instance to this collection. |
| [Add](../../aspose.tasks/ratecollection/add/#add_1)(DateTime, RateType) | Adds a new [`Rate`](../rate/) instance to this collection. |
| [GetEnumerator](../../aspose.tasks/ratecollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/ratecollection/remove/)(Rate) | Removes Rate instance from this collection. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist)() | Converts the `RateCollection` object to a list of [`Rate`](../rate/) objects. |
| [ToList](../../aspose.tasks/ratecollection/tolist/#tolist_1)(RateType) | Converts the `RateCollection` object to a list of [`Rate`](../rate/) objects filtered by specified [`RateType`](../ratetype/) type. |

## Examples

Shows how to work with rate collections.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var resource = project.Resources.Add("Test Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);
resource.Set(Rsc.Work, project.GetDuration(2d, TimeUnitType.Hour));
resource.Set(Rsc.StandardRate, 20m);

var rate1 = resource.Rates.Add(new DateTime(2019, 1, 1, 8, 0, 0));
rate1.RatesTo = new DateTime(2019, 11, 11, 17, 0, 0);
rate1.StandardRate = 5m;
rate1.StandardRateFormat = RateFormatType.Hour;

var rate2 = resource.Rates.Add(new DateTime(2019, 11, 12, 8, 0, 0), RateType.B);
rate2.RatesTo = new DateTime(2019, 12, 31, 17, 0, 0);
rate2.StandardRate = 10m;
rate2.StandardRateFormat = RateFormatType.Hour;

Console.WriteLine("Print rates of '{0}' resource: ", resource.Rates.ParentResource.Get(Rsc.Name));
Console.WriteLine("Count of rates: {0}", resource.Rates.Count);
Console.WriteLine("Is rate collection read-only: {0}", resource.Rates.IsReadOnly);
foreach (KeyValuePair<RateType, RateByDateCollection> sortedRates in resource.Rates)
{
    foreach (KeyValuePair<DateTime, Rate> pair in sortedRates.Value)
    {
        var rate = pair.Value;
        Console.WriteLine("Rates From: " + rate.RatesFrom);
        Console.WriteLine("Rates To: " + rate.RatesTo);
        Console.WriteLine("Rate Table: " + rate.RateTable);
        Console.WriteLine();
    }
}

// get the latest rate by index access
var rateToUpdate = resource.Rates[RateType.B][new DateTime(2019, 11, 12, 8, 0, 0)];
rateToUpdate.RatesTo = new DateTime(2020, 12, 31, 17, 0, 0);
Console.WriteLine("Rates From: " + rateToUpdate.RatesFrom);
Console.WriteLine("Rates To: " + rateToUpdate.RatesTo);

// ...
// work with rates
// ...

// remove all rates of type A
List<Rate> rates = resource.Rates.ToList(RateType.A);
for (var i = 0; i < rates.Count; i++)
{
    var rateToRemove = rates[i];
    resource.Rates.Remove(rateToRemove);
}

// transform the rate collection into a flat list
Console.WriteLine("Iterate over the rates after remove the A-typed values: ");
List<Rate> list = resource.Rates.ToList();
foreach (var rt in list)
{
    Console.WriteLine("Rates From: " + rt.RatesFrom);
    Console.WriteLine("Rates To: " + rt.RatesTo);
    Console.WriteLine("Rate Table: " + rt.RateTable);
}
```

### See Also

* enum [RateType](../ratetype/)
* class [RateByDateCollection](../ratebydatecollection/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


