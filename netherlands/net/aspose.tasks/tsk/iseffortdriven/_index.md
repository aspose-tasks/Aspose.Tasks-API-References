---
title: "Tsk.IsEffortDriven"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of de planning voor de taak een effortdriven scheduling is"
type: docs
weight: 570
url: /nl/net/aspose.tasks/tsk/iseffortdriven/
---
## Tsk.IsEffortDriven field

Bepaalt of de planning voor de taak inspanningsgebaseerd is.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEffortDriven;
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


