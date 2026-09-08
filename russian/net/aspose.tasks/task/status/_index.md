---
title: "Task.Status"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает статус задачи"
type: docs
weight: 1160
url: /ru/net/aspose.tasks/task/status/
---
## Task.Status property

Получает статус задачи.

```csharp
public TaskStatus Status { get; }
```

## Примеры

Показывает, как получить статус задачи.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// Дата статуса проекта должна быть установлена, так как расчёт статуса использует дату статуса.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### См. также

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


