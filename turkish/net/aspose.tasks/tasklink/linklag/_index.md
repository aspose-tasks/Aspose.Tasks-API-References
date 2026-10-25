---
title: "TaskLink.LinkLag"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskLink özelliği. Dakikanın onda biri ya da yüzde olarak gecikmeyi alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks/tasklink/linklag/
---
## TaskLink.LinkLag property

Dakikanın onda birinde veya yüzde olarak gecikmeyi alır veya ayarlar.

```csharp
public int LinkLag { get; set; }
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


