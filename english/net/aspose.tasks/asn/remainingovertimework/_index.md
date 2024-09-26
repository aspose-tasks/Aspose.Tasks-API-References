---
title: Asn.RemainingOvertimeWork
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The remaining overtime work scheduled to complete an assignment
type: docs
weight: 450
url: /net/aspose.tasks/asn/remainingovertimework/
---
## Asn.RemainingOvertimeWork field

The remaining overtime work scheduled to complete an assignment.

```csharp
public static readonly Key<Duration, AsnKey> RemainingOvertimeWork;
```

## Examples

Shows how to read overtime/remaining works/costs of an assignment.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// Print assignment overtimes
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


