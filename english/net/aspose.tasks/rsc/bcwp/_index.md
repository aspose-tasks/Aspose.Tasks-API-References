---
title: Rsc.BCWP
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The budgeted cost of a work performed by a resource for the project todate
type: docs
weight: 140
url: /net/aspose.tasks/rsc/bcwp/
---
## Rsc.BCWP field

The budgeted cost of a work performed by a resource for the project to-date.

```csharp
public static readonly Key<double, RscKey> BCWP;
```

## Examples

Shows how to read resource costs.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// Display all resources costs
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


