---
title: "TaskUtils.Apply"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskUtils. Applique l'algorithme spécifié à chaque tâche d'un arbre"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/taskutils/apply/
---
## TaskUtils.Apply method

Applique l'algorithme spécifié à chaque tâche d'un arbre.

```csharp
public static void Apply(Task root, ITreeAlgorithm<Task> alg, int level)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| root | Tâche | Racine de l'arbre |
| alg | ITreeAlgorithm`1 | Algorithme appliqué. |
| niveau | Int32 | Niveau de la tâche racine. |

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

* class [Task](../../../aspose.tasks/task/)
* interface [ITreeAlgorithm&lt;T&gt;](../../itreealgorithm-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


