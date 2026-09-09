---
title: "Sınıf TaskLink"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskLink sınıfı. Bir öncül bağlantıyı temsil eder"
type: docs
weight: 2410
url: /tr/net/aspose.tasks/tasklink/
---
## TaskLink class

Bir önceki görev bağlantısını temsil eder.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | Harici öncül projeyi alır veya ayarlar. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | Bir öncülün başka bir projenin parçası olup olmadığını belirten bir değeri alır veya ayarlar. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | Gecikme formatını ifade etmek için kullanılan biçimi alır veya ayarlar. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | Dakikanın onda birinde veya yüzde olarak gecikmeyi alır veya ayarlar. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | LagFormat'a bağlı olarak gecikme süresini alır veya ayarlar. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | Bir bağlantının türünü alır veya ayarlar. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | Öncül görevi alır veya ayarlar. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | Sonraki görevi alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | `TaskLink` sınıfının örneği için bir hash kod değeri döndürür. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | Bir TaskLink'in dize temsili döndürür. Temsilin tam detayları belirtilmemiştir ve değişebilir. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


