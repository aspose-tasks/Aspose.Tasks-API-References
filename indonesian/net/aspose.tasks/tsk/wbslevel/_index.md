---
title: "Tsk.WBSLevel"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Tingkat WBS paling kanan dari sebuah tugas"
type: docs
weight: 1140
url: /id/net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

Level WBS paling kanan dari tugas.

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
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


