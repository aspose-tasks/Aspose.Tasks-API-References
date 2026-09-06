---
title: "Asn.OvertimeCost"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. La somme du coût réel et restant des heures supplémentaires d'une affectation"
type: docs
weight: 370
url: /fr/net/aspose.tasks/asn/overtimecost/
---
## Asn.OvertimeCost field

Le total du coût réel et restant des heures supplémentaires d'une affectation.

```csharp
public static readonly Key<decimal, AsnKey> OvertimeCost;
```

## Exemples

Montre comment lire les heures supplémentaires / travaux restants / coûts d'une affectation.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// Imprimer les heures supplémentaires d'affectation
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

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


