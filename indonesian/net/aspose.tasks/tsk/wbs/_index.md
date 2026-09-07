---
title: "Tsk.WBS"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Kode struktur rincian kerja WBS"
type: docs
weight: 1130
url: /id/net/aspose.tasks/tsk/wbs/
---
## Tsk.WBS field

Kode struktur rincian kerja (WBS).

```csharp
public static readonly Key<string, TaskKey> WBS;
```

## Contoh

Menampilkan cara membaca kode WBS tugas.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Mengurai semua tugas yang dikumpulkan
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


