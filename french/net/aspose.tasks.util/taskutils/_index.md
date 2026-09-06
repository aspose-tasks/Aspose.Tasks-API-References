---
title: "Classe TaskUtils"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Util.TaskUtils classe. Classe d'assistance qui fournit des opérations utiles avec les tâches"
type: docs
weight: 2770
url: /fr/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

Classe d'assistance qui fournit des opérations utiles avec les tâches.

```csharp
public static class TaskUtils
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | Applique l'algorithme spécifié à chaque tâche d'un arbre. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | Construit un nouvel arbre de tâches qui satisfont la condition. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | Trouve une tâche qui satisfait la condition dans un arbre de tâches. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | Calcule récursivement le nombre de sous‑tâches d'une tâche à tous les niveaux. |

## Exemples

Montre comment travailler avec un algorithme d'arbre.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// rassembler toutes les tâches du projet
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// travailler avec les tâches comme avec une liste simple
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### Voir aussi

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


