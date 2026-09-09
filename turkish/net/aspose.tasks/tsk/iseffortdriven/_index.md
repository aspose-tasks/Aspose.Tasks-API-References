---
title: "Tsk.IsEffortDriven"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Görevin zamanlamasının çaba odaklı olup olmadığını belirler"
type: docs
weight: 570
url: /tr/net/aspose.tasks/tsk/iseffortdriven/
---
## Tsk.IsEffortDriven field

Görev için zamanlamanın çaba odaklı (effort-driven) olup olmadığını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEffortDriven;
```

## Örnekler

Kritik ve/veya çaba odaklı görevlerin nasıl bulunacağını gösterir.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Toplanan tüm görevleri ayrıştır
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


