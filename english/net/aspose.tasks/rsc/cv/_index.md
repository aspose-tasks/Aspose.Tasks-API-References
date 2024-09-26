---
title: Rsc.CV
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The earned value cost variance through the project status date. CV is the difference between the tasks BCWP budgeted cost of work performed and ACWP actual cost of work performed
type: docs
weight: 270
url: /net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

The earned value cost variance, through the project status date. CV is the difference between the task's BCWP (budgeted cost of work performed) and ACWP (actual cost of work performed).

```csharp
public static readonly Key<double, RscKey> CV;
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


