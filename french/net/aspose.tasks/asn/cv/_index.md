---
title: "Asn.CV"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. La variance du coût de la valeur acquise. CV est la différence entre le BCWP (coût budgété du travail effectué) de l'affectation et l'ACWP (coût réel du travail effectué)."
type: docs
weight: 220
url: /fr/net/aspose.tasks/asn/cv/
---
## Asn.CV field

La variance de coût de la valeur acquise. CV est la différence entre le BCWP (coût budgété du travail effectué) de l'affectation et l'ACWP (coût réel du travail effectué).

```csharp
public static readonly Key<double, AsnKey> CV;
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


