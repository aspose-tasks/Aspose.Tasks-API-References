---
title: "TaskLink.SuccTask"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskLink özelliği. Sonraki görevi alır veya ayarlar"
type: docs
weight: 80
url: /tr/net/aspose.tasks/tasklink/succtask/
---
## TaskLink.SuccTask property

Sonraki görevi alır veya ayarlar.

```csharp
public Task SuccTask { get; set; }
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


