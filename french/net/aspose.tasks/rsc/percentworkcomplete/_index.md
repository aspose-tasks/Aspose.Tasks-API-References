---
title: "Rsc.PercentWorkComplete"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le pourcentage de travail accompli sur l’ensemble des tâches"
type: docs
weight: 550
url: /fr/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

Le pourcentage de travail accompli pour toutes les tâches.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## Exemples

Montre comment lire le pourcentage de travail accompli d’une ressource.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// Afficher le pourcentage d’achèvement du travail pour toutes les ressources
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


