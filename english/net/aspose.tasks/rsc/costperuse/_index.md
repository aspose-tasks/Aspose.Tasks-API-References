---
title: Rsc.CostPerUse
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The cost that accrues every time that a resource is used
type: docs
weight: 240
url: /net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

The cost that accrues every time that a resource is used.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## Examples

Shows how to read/write Rsc.CostPerUse property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


