---
title: "Tsk.ActualCost"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Kaynakların görevlerinde zaten gerçekleştirdiği çalışmalar ve görevle ilişkili diğer kaydedilmiş maliyetler için ortaya çıkan maliyetler"
type: docs
weight: 20
url: /tr/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

Kaynakların görevlerinde zaten yaptığı iş için oluşan maliyetler, görevle ilişkili diğer kaydedilmiş maliyetlerle birlikte.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


