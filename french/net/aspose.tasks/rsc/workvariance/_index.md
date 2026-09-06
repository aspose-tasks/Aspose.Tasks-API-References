---
title: "Rsc.WorkVariance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. La différence entre le travail de référence d’une ressource et le travail actuellement planifié"
type: docs
weight: 710
url: /fr/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

La différence entre le travail de référence d'une ressource et le travail actuellement prévu.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## Exemples

Montre comment lire la variance du travail de la ressource.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


