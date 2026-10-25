---
title: "Tsk.Priority"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Уровень важности, присвоенный задаче, который, в свою очередь, указывает, насколько легко задача или назначение могут быть отложены или разделены при выравнивании ресурсов"
type: docs
weight: 930
url: /ru/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

Уровень важности задачи, который, в свою очередь, указывает, насколько легко задача или назначение могут быть отложены или разбиты во время выравнивания ресурсов.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## Примеры

Показывает, как прочитать приоритет задачи.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Отобразить приоритеты для всех задач
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


