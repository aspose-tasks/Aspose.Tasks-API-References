---
title: Rsc.RemainingCost
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The remaining scheduled expense that will be incurred in completing the remaining scheduled work
type: docs
weight: 580
url: /net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

The remaining scheduled expense that will be incurred in completing the remaining scheduled work.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## Examples

Shows how to read/write Rsc.RemainingCost property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


