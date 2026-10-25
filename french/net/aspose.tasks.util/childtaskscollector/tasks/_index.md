---
title: "ChildTasksCollector.Tasks"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété ChildTasksCollector. Obtient une liste des tâches d'objets enfants collectées"
type: docs
weight: 20
url: /fr/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

Obtient une liste d'objets enfants collectés (tâches).

```csharp
public List<Task> Tasks { get; }
```

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

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


