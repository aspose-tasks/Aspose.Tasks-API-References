---
title: "Asn.CostVariance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. La différence entre le coût de référence et le coût total d'une affectation"
type: docs
weight: 200
url: /fr/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

La différence entre le coût de référence et le coût total d'une affectation.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
```

## Exemples

Montre comment lire les écarts d'affectation.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// Imprimer les écarts d'affectation
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


