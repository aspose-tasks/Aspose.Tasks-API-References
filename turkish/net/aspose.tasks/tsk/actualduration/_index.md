---
title: "Tsk.ActualDuration"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Planlanan süre ve mevcut kalan iş ya da tamamlanma yüzdesine dayalı bir görevin gerçek çalışma süresi."
type: docs
weight: 30
url: /tr/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

Planlanan süre ve mevcut kalan iş ya da yüzde tamamlanmaya dayalı olarak bir görevin gerçek çalışma süresi aralığı.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
```

## Örnekler

Görevin gerçek özelliklerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Toplanan tüm görevleri ayrıştır
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


