---
title: "Asn.SV"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. De earned value schema-variantie tot de projectstatusdatum. Schema-variantie SV is het verschil tussen de BCWP en de BCWS"
type: docs
weight: 540
url: /nl/net/aspose.tasks/asn/sv/
---
## Asn.SV field

De verdiende-waarde planningsvariantie tot de projectstatusdatum. Planningsvariantie (SV) is het verschil tussen de BCWP en de BCWS.

```csharp
public static readonly Key<double, AsnKey> SV;
```

## Voorbeelden

Toont hoe de kostwaarden van een toewijzing te lezen zijn.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// Print resource-toewijzingskosten
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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


