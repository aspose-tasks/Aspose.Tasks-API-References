---
title: "Tsk.OvertimeCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir kaynak için tüm atanan görevlerde veya bir kaynak atamasında bir görevin toplam fazla mesai maliyeti"
type: docs
weight: 860
url: /tr/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

Bir görev için, bir kaynak için tüm atanan görevlerdeki veya bir kaynak ataması için toplam fazla mesai maliyeti.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


