---
title: Rsc.ActualCost
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Costs incurred for work already performed by resources on their tasks along with any other recorded costs associated with the task
type: docs
weight: 30
url: /net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

Costs incurred for work already performed by resources on their tasks, along with any other recorded costs associated with the task.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## Examples

Shows how to read/write Rsc.ActualCost property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


