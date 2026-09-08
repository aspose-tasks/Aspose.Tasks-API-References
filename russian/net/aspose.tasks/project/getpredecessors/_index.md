---
title: "Project.GetPredecessors"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Project. Возвращает коллекцию ссылок задач, которые являются предшественниками указанной задачи"
type: docs
weight: 1120
url: /ru/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

Возвращает коллекцию связей задач, которые являются предшественниками указанной задачи.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| задача | Задача | Задача, для которой нужно получить предшественников. |

### Возвращаемое значение

Список предшественников [`TaskLink`](../../tasklink/).

## Примеры

Показывает, как получить предшественников для конкретной задачи.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// Отобразить имена предшествующей и последующей задач.
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### См. также

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


