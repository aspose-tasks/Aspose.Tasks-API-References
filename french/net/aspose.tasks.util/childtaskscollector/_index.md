---
title: "Classe ChildTasksCollector"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Util.ChildTasksCollector. Collecte toutes les tâches enfants"
type: docs
weight: 2690
url: /fr/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

Collecte toutes les sous‑tâches.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | Initialise une nouvelle instance de la classe `ChildTasksCollector`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | Obtient une liste d'objets enfants collectés (tâches). |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | Traite l'objet spécifié. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

## Exemples

Montre comment itérer sur toutes les tâches d'un projet sous forme de liste simple.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analyser toutes les tâches collectées
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Voir aussi

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


