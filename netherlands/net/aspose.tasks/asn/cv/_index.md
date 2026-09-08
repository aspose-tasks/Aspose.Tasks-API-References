---
title: "Asn.CV"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. De kostvariatie van de verdiende waarde. CV is het verschil tussen de BCWP (begrote kosten van uitgevoerd werk) van de toewijzing en de ACWP (werkelijke kosten van uitgevoerd werk)."
type: docs
weight: 220
url: /nl/net/aspose.tasks/asn/cv/
---
## Asn.CV field

De earned value kostenvariantie. CV is het verschil tussen de BCWP (begrote kosten van uitgevoerde werkzaamheden) en de ACWP (werkelijke kosten van uitgevoerde werkzaamheden) van de opdracht.

```csharp
public static readonly Key<double, AsnKey> CV;
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


