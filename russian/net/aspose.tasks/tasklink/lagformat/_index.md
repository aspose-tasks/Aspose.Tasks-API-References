---
title: "TaskLink.LagFormat"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TaskLink. Возвращает или задает формат представления задержки"
type: docs
weight: 30
url: /ru/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

Получает или задает формат представления задержки.

```csharp
public TimeUnitType LagFormat { get; set; }
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

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


