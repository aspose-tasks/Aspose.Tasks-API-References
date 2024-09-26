---
title: Rsc.OvertimeCost
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The total overtime cost for a resource on all assigned tasks
type: docs
weight: 500
url: /net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

The total overtime cost for a resource on all assigned tasks.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## Examples

Shows how to read resource overtime values.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Display overtime related parameters for all resources
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


