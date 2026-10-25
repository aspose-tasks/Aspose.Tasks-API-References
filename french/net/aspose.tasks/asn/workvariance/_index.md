---
title: "Asn.WorkVariance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. La différence entre le travail de référence d'une tâche et le travail actuellement programmé"
type: docs
weight: 620
url: /fr/net/aspose.tasks/asn/workvariance/
---
## Asn.WorkVariance field

La différence entre le travail de référence d'une tâche et le travail actuellement planifié.

```csharp
public static readonly Key<Duration, AsnKey> WorkVariance;
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


