---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор ChildTasksCollector. Инициализирует новый экземпляр класса ChildTasksCollector"
type: docs
weight: 10
url: /ru/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

Инициализирует новый экземпляр класса [`ChildTasksCollector`](../).

```csharp
public ChildTasksCollector()
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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


