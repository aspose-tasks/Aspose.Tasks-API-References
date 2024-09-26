---
title: Asn.FinishVariance
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The variance of an assignment finish date from a baseline finish date
type: docs
weight: 250
url: /net/aspose.tasks/asn/finishvariance/
---
## Asn.FinishVariance field

The variance of an assignment finish date from a baseline finish date.

```csharp
public static readonly Key<Duration, AsnKey> FinishVariance;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


