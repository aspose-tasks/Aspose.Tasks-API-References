---
title: "Tsk.OutlineNumber"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Номер, представляющий позицию задачи в иерархической структуре контура"
type: docs
weight: 850
url: /ru/net/aspose.tasks/tsk/outlinenumber/
---
## Tsk.OutlineNumber field

Число, представляющее позицию задачи в иерархической структуре.

```csharp
public static readonly Key<string, TaskKey> OutlineNumber;
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


