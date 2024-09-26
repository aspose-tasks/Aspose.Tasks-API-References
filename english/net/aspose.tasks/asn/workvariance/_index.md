---
title: Asn.WorkVariance
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The difference between baseline work of a task and the currently scheduled work
type: docs
weight: 620
url: /net/aspose.tasks/asn/workvariance/
---
## Asn.WorkVariance field

The difference between baseline work of a task and the currently scheduled work.

```csharp
public static readonly Key<Duration, AsnKey> WorkVariance;
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


