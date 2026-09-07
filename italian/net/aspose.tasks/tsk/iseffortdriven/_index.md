---
title: "Tsk.IsEffortDriven"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se la programmazione dell'attività è basata sullo sforzo"
type: docs
weight: 570
url: /it/net/aspose.tasks/tsk/iseffortdriven/
---
## Tsk.IsEffortDriven field

Determina se la pianificazione dell'attività è basata sul carico di lavoro.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEffortDriven;
```

## Esempi

Mostra come trovare attività critiche e/o basate sullo sforzo.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizza tutti i task raccolti
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


