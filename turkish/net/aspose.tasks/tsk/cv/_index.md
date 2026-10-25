---
title: "Tsk.CV"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görev için temel maliyet ile toplam maliyet arasındaki fark. Maliyet Varyansı  Maliyet  Temel Maliyet"
type: docs
weight: 260
url: /tr/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

Bir görev için temel maliyet ile toplam maliyet arasındaki fark. Cost Variance = Cost - Baseline Cost

```csharp
public static readonly Key<double, TaskKey> CV;
```

## Örnekler

Görev maliyet değerlerinin nasıl okunacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


