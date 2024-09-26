---
title: Asn.RemainingOvertimeCost
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The remaining projected overtime cost of completing an assignment
type: docs
weight: 440
url: /net/aspose.tasks/asn/remainingovertimecost/
---
## Asn.RemainingOvertimeCost field

The remaining projected overtime cost of completing an assignment.

```csharp
public static readonly Key<decimal, AsnKey> RemainingOvertimeCost;
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
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


