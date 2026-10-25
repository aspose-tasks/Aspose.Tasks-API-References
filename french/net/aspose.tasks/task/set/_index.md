---
title: "Task.Set"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Associe la propriété spécifiée à la valeur spécifiée dans ce conteneur"
type: docs
weight: 1410
url: /fr/net/aspose.tasks/task/set/
---
## Task.Set&lt;T&gt; method

Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur.

```csharp
public void Set<T>(Key<T, TaskKey> key, T val)
```

| Paramètre | Description |
| --- | --- |
| T | le type de la valeur mappée. |
| key | la clé de propriété spécifiée. [`Tsk`](../../tsk/) pour obtenir la clé de propriété. |
| val | la valeur. |

## Exemples

Montre comment obtenir/définir les propriétés de la tâche.

```csharp
var project = new Project();

// Ajouter une tâche et définir les propriétés de la tâche
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analyser toutes les tâches collectées
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


