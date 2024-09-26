---
title: Asn.OvertimeCost
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The sum of the actual and remaining overtime cost of an assignment
type: docs
weight: 370
url: /net/aspose.tasks/asn/overtimecost/
---
## Asn.OvertimeCost field

The sum of the actual and remaining overtime cost of an assignment.

```csharp
public static readonly Key<decimal, AsnKey> OvertimeCost;
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


