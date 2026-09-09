---
title: "Tsk.IsEstimated"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Bir görevin tahmini olup olmadığını belirler."
type: docs
weight: 580
url: /tr/net/aspose.tasks/tsk/isestimated/
---
## Tsk.IsEstimated field

Bir görevin tahmini olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEstimated;
```

## Örnekler

Tahmini ve/veya kilometre taşı görevlerinin nasıl bulunacağını gösterir.

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// Toplanan görevler üzerinde yineleme yapın.
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


