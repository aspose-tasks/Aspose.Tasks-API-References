---
title: "Tsk.IsCritical"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk field. Bepaalt of een taak zich op het kritieke pad bevindt"
type: docs
weight: 560
url: /nl/net/aspose.tasks/tsk/iscritical/
---
## Tsk.IsCritical field

Bepaalt of een taak zich op het kritieke pad bevindt.

```csharp
public static readonly Key<NullableBool, TaskKey> IsCritical;
```

## Voorbeelden

Toont hoe kritieke en/of effort-driven taken te vinden.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Alle verzamelde taken doorlopen
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


