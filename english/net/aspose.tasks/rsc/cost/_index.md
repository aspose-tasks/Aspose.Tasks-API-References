---
title: Rsc.Cost
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The total scheduled or projected cost for a resource based on costs already incurred for work performed by resources assigned to the tasks in addition to the costs planned for the remaining work
type: docs
weight: 220
url: /net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

The total scheduled or projected cost for a resource, based on costs already incurred for work performed by resources assigned to the tasks, in addition to the costs planned for the remaining work.

```csharp
public static readonly Key<decimal, RscKey> Cost;
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


