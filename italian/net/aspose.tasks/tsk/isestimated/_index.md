---
title: "Tsk.IsEstimated"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se un'attività è stimata"
type: docs
weight: 580
url: /it/net/aspose.tasks/tsk/isestimated/
---
## Tsk.IsEstimated field

Determina se un'attività è stimata.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEstimated;
```

## Esempi

Mostra come trovare attività stimate e/o traguardi.

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// Itera sulle attività raccolte
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


