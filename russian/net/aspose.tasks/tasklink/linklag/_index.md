---
title: "TaskLink.LinkLag"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TaskLink. Возвращает или задает задержку в десятых долях минуты или в процентах"
type: docs
weight: 40
url: /ru/net/aspose.tasks/tasklink/linklag/
---
## TaskLink.LinkLag property

Получает или задает задержку в десятых долях минуты или в процентах.

```csharp
public int LinkLag { get; set; }
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


