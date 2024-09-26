---
title: Resource.Baselines
second_title: Aspose.Tasks for .NET API Reference
description: Resource property. Gets a BaselineCollection instance for this object. The baseline values for a resource
type: docs
weight: 160
url: /net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

Gets a BaselineCollection instance for this object. The baseline values for a resource.

```csharp
public BaselineCollection Baselines { get; }
```

## Examples

Shows how to read resource's baselines.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### See Also

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


