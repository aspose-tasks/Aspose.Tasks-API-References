---
title: "Tsk.OutlineLevel"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Уровень структуры задачи"
type: docs
weight: 840
url: /ru/net/aspose.tasks/tsk/outlinelevel/
---
## Tsk.OutlineLevel field

Уровень структуры задачи.

```csharp
public static readonly Key<int, TaskKey> OutlineLevel;
```

## Примеры

Показывает, как читать свойства структуры задачи.

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Проанализировать все собранные задачи
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


