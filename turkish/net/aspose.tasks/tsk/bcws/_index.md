---
title: "Tsk.BCWS"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Durum tarihine veya bugünkü tarihe kadar birikimli zaman aşamalı temel maliyetler"
type: docs
weight: 130
url: /tr/net/aspose.tasks/tsk/bcws/
---
## Tsk.BCWS field

Durum tarihine veya bugünkü tarihe kadar olan kümülatif zaman aşamalı temel maliyetler.

```csharp
public static readonly Key<double, TaskKey> BCWS;
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


