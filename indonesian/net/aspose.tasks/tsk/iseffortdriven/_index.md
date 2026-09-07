---
title: "Tsk.IsEffortDriven"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah penjadwalan tugas menggunakan penjadwalan berbasis upaya"
type: docs
weight: 570
url: /id/net/aspose.tasks/tsk/iseffortdriven/
---
## Tsk.IsEffortDriven field

Menentukan apakah penjadwalan tugas menggunakan penjadwalan berbasis upaya.

```csharp
public static readonly Key<NullableBool, TaskKey> IsEffortDriven;
```

## Contoh

Menampilkan cara menemukan tugas kritis dan/atau berbasis upaya.

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Mengurai semua tugas yang dikumpulkan
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


