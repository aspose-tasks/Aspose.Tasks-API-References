---
title: Rsc.ActualOvertimeCost
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Costs incurred for overtime work already performed on tasks by assigned resources
type: docs
weight: 40
url: /net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

Costs incurred for overtime work already performed on tasks by assigned resources.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## Examples

Shows how to read/write Rsc.ActualOvertimeCost property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


