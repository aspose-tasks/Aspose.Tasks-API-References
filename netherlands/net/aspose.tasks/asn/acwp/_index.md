---
title: "Asn.ACWP"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn veld. De werkelijke kosten van een uitgevoerde taak op een toewijzing tot op heden"
type: docs
weight: 90
url: /nl/net/aspose.tasks/asn/acwp/
---
## Asn.ACWP field

De werkelijke kosten van tot nu toe uitgevoerd werk op een toewijzing.

```csharp
public static readonly Key<double, AsnKey> ACWP;
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


