---
title: "Tsk.ACWP"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Proje durum tarihine veya bugünün tarihine kadar bir görevde zaten yapılan iş için oluşan maliyetler"
type: docs
weight: 110
url: /tr/net/aspose.tasks/tsk/acwp/
---
## Tsk.ACWP field

Bir görevde zaten yapılan iş için oluşan maliyetler, proje durum tarihine veya bugünkü tarihe kadar.

```csharp
public static readonly Key<double, TaskKey> ACWP;
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


