---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur ChildTasksCollector. Initialise une nouvelle instance de la classe ChildTasksCollector"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

Initialise une nouvelle instance de la classe [`ChildTasksCollector`](../).

```csharp
public ChildTasksCollector()
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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


