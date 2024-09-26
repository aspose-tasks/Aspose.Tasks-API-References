---
title: Asn.BCWS
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The budgeted cost of a work on assignment
type: docs
weight: 130
url: /net/aspose.tasks/asn/bcws/
---
## Asn.BCWS field

The budgeted cost of a work on assignment.

```csharp
public static readonly Key<double, AsnKey> BCWS;
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


