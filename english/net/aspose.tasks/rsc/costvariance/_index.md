---
title: Rsc.CostVariance
second_title: Aspose.Tasks for .NET API Reference
description: Rsc field. The difference between the baseline cost and total cost for a resource
type: docs
weight: 250
url: /net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

The difference between the baseline cost and total cost for a resource.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## Examples

Shows how to read/write Rsc.CostVariance property.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


