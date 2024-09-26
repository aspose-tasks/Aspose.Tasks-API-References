---
title: Asn.SV
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The earned value schedule variance through the project status date. Schedule variance SV is the difference between the BCWP and the BCWS
type: docs
weight: 540
url: /net/aspose.tasks/asn/sv/
---
## Asn.SV field

The earned value schedule variance, through the project status date. Schedule variance (SV) is the difference between the BCWP and the BCWS.

```csharp
public static readonly Key<double, AsnKey> SV;
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


