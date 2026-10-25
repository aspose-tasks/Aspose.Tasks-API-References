---
title: "TaskLink.LagFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskLink özelliği. Gecikme biçimini ifade etmek için formatı alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

Gecikme formatını ifade etmek için kullanılan biçimi alır veya ayarlar.

```csharp
public TimeUnitType LagFormat { get; set; }
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

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


