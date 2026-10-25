---
title: "Asn.FinishVariance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. La variance de la date de fin d'une affectation par rapport à la date de fin de référence"
type: docs
weight: 250
url: /fr/net/aspose.tasks/asn/finishvariance/
---
## Asn.FinishVariance field

La variance de la date de fin d'une affectation par rapport à une date de fin de référence.

```csharp
public static readonly Key<Duration, AsnKey> FinishVariance;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


