---
title: "ChildTasksCollector.Alg"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ChildTasksCollector. Обрабатывает указанный объект"
type: docs
weight: 30
url: /ru/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

Обрабатывает указанный объект.

```csharp
public override void Alg(Task el, int level)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| el | Задача | Объект для обработки. |
| уровень | Int32 | Уровень узла дерева. |

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


