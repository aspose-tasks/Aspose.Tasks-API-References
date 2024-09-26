---
title: Asn.CostVariance
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The difference between the baseline cost and total cost for an assignment
type: docs
weight: 200
url: /net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

The difference between the baseline cost and total cost for an assignment.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
```

## Examples

Shows how to read assignment's variances.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// Print assignment variances
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


