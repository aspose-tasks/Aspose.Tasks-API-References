---
title: "TaskLink.PredTask"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TaskLink. Возвращает или задает предшествующую задачу"
type: docs
weight: 70
url: /ru/net/aspose.tasks/tasklink/predtask/
---
## TaskLink.PredTask property

Получает или задает предшествующую задачу.

```csharp
public Task PredTask { get; set; }
```

## Примеры

Показывает, как читать ссылки задач проекта.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Отобразить имена предшествующей и последующей задач.
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### См. также

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


