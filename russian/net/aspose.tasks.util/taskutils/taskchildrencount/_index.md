---
title: "TaskUtils.TaskChildrenCount"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskUtils. Рекурсивно вычисляет количество дочерних задач на всех уровнях"
type: docs
weight: 40
url: /ru/net/aspose.tasks.util/taskutils/taskchildrencount/
---
## TaskUtils.TaskChildrenCount method

Рекурсивно вычисляет количество дочерних задач задачи на всех уровнях.

```csharp
public static int TaskChildrenCount(Task task)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| задача | Задача | Задача, для которой вычисляются дочерние задачи. |

### Возвращаемое значение

Количество дочерних задач.

## Примеры

Показывает, как использовать &lt;see cref="Aspose.Tasks.Util.TaskUtils.TaskChildrenCount" /&gt; метод.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// рекурсивно вычисляет количество дочерних задач на всех уровнях
var count = TaskUtils.TaskChildrenCount(project.RootTask);

Console.WriteLine("Number of tasks: " + count);
```

### См. также

* class [Task](../../../aspose.tasks/task/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


