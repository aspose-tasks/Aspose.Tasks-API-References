---
title: Class BaselineCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.BaselineCollection class. Represents a collection of Baseline objects
type: docs
weight: 120
url: /net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

Represents a collection of [`Baseline`](../baseline/) objects.

```csharp
public class BaselineCollection : IList<Baseline>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | Gets the number of objects contained in this BaselineCollection object. |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | Returns the element at the specified index. |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | Gets the parent [`Resource`](../resource/) for this collection. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | This is the stub implementation of ICollection's Add method, that only throws NotSupportedException |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | Removes baseline from this collection. |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | Converts the BaselineCollection object to a list of [`Baseline`](../baseline/) objects. |

## Examples

Shows how to work with baseline collections.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// read baseline information
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### See Also

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


