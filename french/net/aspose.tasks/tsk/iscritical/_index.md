---
title: "Tsk.IsCritical"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si une tâche se trouve sur le chemin critique"
type: docs
weight: 560
url: /fr/net/aspose.tasks/tsk/iscritical/
---
## Tsk.IsCritical field

Détermine si une tâche se trouve sur le chemin critique.

```csharp
public static readonly Key<NullableBool, TaskKey> IsCritical;
```

## Exemples

Montre comment trouver les tâches critiques et/ou basées sur l'effort.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analyser toutes les tâches collectées
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


