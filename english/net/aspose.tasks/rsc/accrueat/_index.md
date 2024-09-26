---
title: Rsc.AccrueAt
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Determines how and when resource standard and overtime costs are to be charged or accrued to the cost of a task
type: docs
weight: 10
url: /net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

Determines how and when resource standard and overtime costs are to be charged, or accrued, to the cost of a task.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## Examples

Shows how to read/write Rsc.AccrueAt property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


