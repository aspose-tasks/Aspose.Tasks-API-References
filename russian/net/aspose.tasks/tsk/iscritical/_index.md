---
title: "Tsk.IsCritical"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, находится ли задача на критическом пути"
type: docs
weight: 560
url: /ru/net/aspose.tasks/tsk/iscritical/
---
## Tsk.IsCritical field

Определяет, находится ли задача на критическом пути.

```csharp
public static readonly Key<NullableBool, TaskKey> IsCritical;
```

## Примеры

Показывает, как находить критические и/или задачи с планированием на основе усилий.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Проанализировать все собранные задачи
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


