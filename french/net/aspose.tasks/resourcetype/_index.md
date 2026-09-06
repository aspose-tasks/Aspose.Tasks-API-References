---
title: "Enum ResourceType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.ResourceType. Spécifie le type d'une ressource"
type: docs
weight: 1800
url: /fr/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

Spécifie le type d'une ressource.

```csharp
public enum ResourceType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Material | `0` | Indique le type de ressource Matériel. |
| Work | `1` | Indique le type de ressource Travail. |
| Cost | `2` | Indique le type de ressource Coût. |

## Exemples

Montre comment travailler avec les types de ressources.

```csharp
var project = new Project();

// ajouter une ressource de travail
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// ajouter une ressource matérielle
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// ajouter une ressource matérielle
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// travailler avec les ressources : créer des tâches, assigner des ressources, etc.
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


