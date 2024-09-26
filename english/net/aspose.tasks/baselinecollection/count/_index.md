---
title: BaselineCollection.Count
second_title: Aspose.Tasks for .NET API Reference
description: BaselineCollection property. Gets the number of objects contained in this BaselineCollection object
type: docs
weight: 10
url: /net/aspose.tasks/baselinecollection/count/
---
## BaselineCollection.Count property

Gets the number of objects contained in this BaselineCollection object.

```csharp
public int Count { get; }
```

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

* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


