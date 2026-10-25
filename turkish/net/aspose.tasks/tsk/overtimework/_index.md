---
title: "Tsk.OvertimeWork"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir göreve atanan tüm kaynaklar tarafından yapılması planlanan fazla mesai miktarı"
type: docs
weight: 870
url: /tr/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

Bir göreve atanan tüm kaynaklar tarafından yapılması planlanan fazla mesai miktarı.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## Örnekler

Görev fazla mesailerini okuma nasıl yapılır gösterir.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// Görevler için fazla mesai ve yüzde tamamlama değerlerini okuyun
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // Yüzde tamamlamayı ayarlayın
    task.Set(Tsk.PercentComplete, 100);
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


