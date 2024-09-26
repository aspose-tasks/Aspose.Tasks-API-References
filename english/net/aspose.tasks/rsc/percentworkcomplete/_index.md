---
title: Rsc.PercentWorkComplete
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The percentage of work completed across all tasks
type: docs
weight: 550
url: /net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

The percentage of work completed across all tasks.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## Examples

Shows how to read resource percent work complete.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// Display work percentage completion for all resources
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


