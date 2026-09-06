---
title: "Tsk.IsEffortDriven"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si la planification de la tâche est basée sur l'effort"
type: docs
weight: 570
url: /fr/net/aspose.tasks/tsk/iseffortdriven/
---
## Tsk.IsEffortDriven field

Détermine si la planification de la tâche est basée sur l’effort.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEffortDriven;
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


