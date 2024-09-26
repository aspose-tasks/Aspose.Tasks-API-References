---
title: Rsc.OvertimeWork
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The amount of overtime scheduled to be performed by a resource on a task and charged at the overtime rates of the resources involved
type: docs
weight: 530
url: /net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

The amount of overtime scheduled to be performed by a resource on a task and charged at the overtime rates of the resources involved.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


