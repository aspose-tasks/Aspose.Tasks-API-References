---
title: Prj.SpreadActualCost
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether actual costs are spread to the status date
type: docs
weight: 660
url: /net/aspose.tasks/prj/spreadactualcost/
---
## Prj.SpreadActualCost field

Determines whether actual costs are spread to the status date.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadActualCost;
```

## Examples

Shows how to read/write Prj.SpreadActualCost property.

```csharp
var project = new Project();

project.Set(Prj.SpreadActualCost, true);

Console.WriteLine("Spread Actual Cost: " + project.Get(Prj.SpreadActualCost));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


