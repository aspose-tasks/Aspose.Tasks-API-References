---
title: Asn.StartVariance
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The variance of an assignment start date from a baseline start date
type: docs
weight: 510
url: /net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

The variance of an assignment start date from a baseline start date.

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
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


