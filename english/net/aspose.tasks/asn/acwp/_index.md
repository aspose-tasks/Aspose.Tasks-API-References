---
title: Asn.ACWP
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The actual cost of a work performed on an assignment todate
type: docs
weight: 90
url: /net/aspose.tasks/asn/acwp/
---
## Asn.ACWP field

The actual cost of a work performed on an assignment to-date.

```csharp
public static readonly Key<double, AsnKey> ACWP;
```

## Examples

Shows how to read assignment's cost values.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// Print resource assignment costs
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine(assignment.Get(Asn.Cost));
    Console.WriteLine(assignment.Get(Asn.ACWP));

    // CV = BCWP - ACWP
    Console.WriteLine(assignment.Get(Asn.CV));

    Console.WriteLine(assignment.Get(Asn.BCWP));
    Console.WriteLine(assignment.Get(Asn.BCWS));

    // SV = BCWP - BCWS
    Console.WriteLine(assignment.Get(Asn.SV));
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


