---
title: "Asn.RemainingWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Le travail restant programmé pour terminer une affectation"
type: docs
weight: 460
url: /fr/net/aspose.tasks/asn/remainingwork/
---
## Asn.RemainingWork field

Le travail restant prévu pour terminer une affectation.

```csharp
public static readonly Key<Duration, AsnKey> RemainingWork;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


