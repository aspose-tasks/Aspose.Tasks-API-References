---
title: "ChildTasksCollector.Tasks"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ChildTasksCollector. Получает список задач, собранных у дочерних объектов"
type: docs
weight: 20
url: /ru/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

Получает список собранных дочерних объектов (задач).

```csharp
public List<Task> Tasks { get; }
```

## Примеры

Показывает, как перебрать все задачи в проекте в виде простого списка.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Проанализировать все собранные задачи
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### См. также

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


