---
title: "Tsk.WBSLevel"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le niveau WBS le plus à droite d'une tâche"
type: docs
weight: 1140
url: /fr/net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

Le niveau WBS le plus à droite d'une tâche.

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
```

## Exemples

Montre comment lire les codes WBS d'une tâche.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analyser toutes les tâches collectées
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


