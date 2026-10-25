---
title: "Classe LevelingResult"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Leveling.LevelingResult class. Représente les résultats du nivellement des ressources."
type: docs
weight: 960
url: /fr/net/aspose.tasks.leveling/levelingresult/
---
## LevelingResult class

Représente les résultats du nivellement des ressources.

```csharp
public sealed class LevelingResult
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LevelingResult](levelingresult/)() | Initialise une nouvelle instance de la classe `LevelingResult`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AffectedTasks](../../aspose.tasks.leveling/levelingresult/affectedtasks/) { get; } | Obtient un ensemble de tâches affectées par le nivellement des ressources. |

## Exemples

Montre comment niveler toutes les ressources du projet en utilisant les options par défaut.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingResult = ResourceLeveler.LevelAll(project);

foreach (var task in levelingResult.AffectedTasks)
{
    Console.WriteLine("Task affected by the leveling operation: " + task.Name);
}

project.Save(OutDir + "Software Development Plan.leveled.mpp");
ResourceLeveler.ClearLeveling(project);

Console.WriteLine("Leveling cleared");
```

### Voir aussi

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


