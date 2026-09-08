---
title: "Tsk.IsEstimated"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, является ли задача оценочной."
type: docs
weight: 580
url: /ru/net/aspose.tasks/tsk/isestimated/
---
## Tsk.IsEstimated field

Определяет, является ли задача оценочной.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEstimated;
```

## Примеры

Показывает, как находить оценочные и/или контрольные задачи.

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// Итерировать собранные задачи
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


