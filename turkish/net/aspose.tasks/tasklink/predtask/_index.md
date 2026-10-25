---
title: "TaskLink.PredTask"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskLink özelliği. Önceki görevi alır veya ayarlar"
type: docs
weight: 70
url: /tr/net/aspose.tasks/tasklink/predtask/
---
## TaskLink.PredTask property

Öncül görevi alır veya ayarlar.

```csharp
public Task PredTask { get; set; }
```

## Örnekler

Proje görev bağlantılarını nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Öncül ve sonraki görevlerin adlarını göster
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


