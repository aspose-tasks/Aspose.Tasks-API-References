---
title: "Asn.ACWP"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Le coût réel du travail effectué sur une affectation à ce jour"
type: docs
weight: 90
url: /fr/net/aspose.tasks/asn/acwp/
---
## Asn.ACWP field

Le coût réel d'un travail effectué sur une affectation à ce jour.

```csharp
public static readonly Key<double, AsnKey> ACWP;
```

## Exemples

Montre comment lire les valeurs de coût d'une affectation.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// Imprimer les coûts d'affectation de ressources
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

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


