---
title: "ResourceLeveler.ClearLeveling"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceLeveler. Supprime tout retard de nivellement qui a été précédemment ajouté au projet lors du nivellement des ressources."
type: docs
weight: 10
url: /fr/net/aspose.tasks.leveling/resourceleveler/clearleveling/
---
## ClearLeveling(Project) {#clearleveling}

Supprime tout retard de nivellement qui avait été ajouté précédemment au projet pendant le nivellement des ressources.

```csharp
public static void ClearLeveling(Project project)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| project | Project | Projet dont le nivellement doit être supprimé. |

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

* class [Project](../../../aspose.tasks/project/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)

---

## ClearLeveling(IEnumerable&lt;Task&gt;) {#clearleveling_1}

Supprime tout retard de nivellement qui avait été ajouté précédemment aux tâches spécifiées pendant le nivellement des ressources.

```csharp
public static void ClearLeveling(IEnumerable<Task> tasks)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tâches | IEnumerable`1 | L'énumérable contenant les tâches pour lesquelles le retard de nivellement doit être supprimé. |

### Voir aussi

* class [Task](../../../aspose.tasks/task/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


