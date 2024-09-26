---
title: Rsc.CostCenter
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. Indicates which cost center the costs accrued by the resource should be charged to
type: docs
weight: 230
url: /net/aspose.tasks/rsc/costcenter/
---
## Rsc.CostCenter field

Indicates which cost center the costs accrued by the resource should be charged to.

```csharp
public static readonly Key<string, RscKey> CostCenter;
```

## Examples

Shows how to read/write Rsc.CostCenter property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostCenter, "Center");

Console.WriteLine("Cost Center: " + resource.Get(Rsc.CostCenter));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


