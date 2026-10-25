---
title: "Tsk.IsMilestone"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah sebuah tugas adalah tonggak"
type: docs
weight: 630
url: /id/net/aspose.tasks/tsk/ismilestone/
---
## Tsk.IsMilestone field

Menentukan apakah sebuah tugas merupakan tonggak.

```csharp
public static readonly Key<NullableBool, TaskKey> IsMilestone;
```

## Contoh

Menampilkan cara menemukan tugas yang diperkirakan dan/atau tonggak.

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// Iterasi atas tugas yang dikumpulkan
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


