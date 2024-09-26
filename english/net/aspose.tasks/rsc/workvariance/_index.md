---
title: Rsc.WorkVariance
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The difference between baseline work of a resource and the currently scheduled work
type: docs
weight: 710
url: /net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

The difference between baseline work of a resource and the currently scheduled work.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## Examples

Shows how to read resource work variance.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


