---
title: BaselineCollection.ToList
second_title: Aspose.Tasks for .NET API Reference
description: BaselineCollection method. Converts the BaselineCollection object to a list of Baseline objects
type: docs
weight: 70
url: /net/aspose.tasks/baselinecollection/tolist/
---
## BaselineCollection.ToList method

Converts the BaselineCollection object to a list of [`Baseline`](../../baseline/) objects.

```csharp
public List<Baseline> ToList()
```

### Return Value

List of [`Baseline`](../../baseline/) objects.

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

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


