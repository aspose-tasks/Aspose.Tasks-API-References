---
title: "Tsk.Priority"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tingkat kepentingan yang diberikan pada sebuah tugas yang pada gilirannya menunjukkan seberapa mudah sebuah tugas atau penugasan dapat ditunda atau dibagi selama penyeimbangan sumber daya."
type: docs
weight: 930
url: /id/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

Tingkat pentingnya sebuah tugas, yang pada gilirannya menunjukkan seberapa mudah tugas atau penugasan dapat ditunda atau dibagi selama leveling sumber daya.

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## Contoh

Menampilkan cara membaca prioritas tugas.

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Tampilkan Prioritas untuk semua tugas
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


