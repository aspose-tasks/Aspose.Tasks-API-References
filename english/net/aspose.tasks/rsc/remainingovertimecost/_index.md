---
title: Rsc.RemainingOvertimeCost
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The remaining scheduled overtime expense for a resource
type: docs
weight: 590
url: /net/aspose.tasks/rsc/remainingovertimecost/
---
## Rsc.RemainingOvertimeCost field

The remaining scheduled overtime expense for a resource.

```csharp
public static readonly Key<decimal, RscKey> RemainingOvertimeCost;
```

## Examples

Shows how to read/write Rsc.RemainingOvertimeCost property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeCost, 3);

Console.WriteLine("Remaining Overtime Cost: " + resource.Get(Rsc.RemainingOvertimeCost));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


