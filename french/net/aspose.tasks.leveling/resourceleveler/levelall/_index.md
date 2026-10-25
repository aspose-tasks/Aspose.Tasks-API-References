---
title: "ResourceLeveler.LevelAll"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceLeveler. Nivele les tâches pour toutes les ressources du projet en utilisant les options de nivellement par défaut."
type: docs
weight: 20
url: /fr/net/aspose.tasks.leveling/resourceleveler/levelall/
---
## ResourceLeveler.LevelAll method

Nivele les tâches pour toutes les ressources du projet en utilisant les options de nivellement par défaut.

```csharp
public static LevelingResult LevelAll(Project project)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| project | Project | Projet auquel appliquer le nivellement des ressources. |

### Valeur de retour

Objet contenant les résultats du nivellement des ressources.

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


