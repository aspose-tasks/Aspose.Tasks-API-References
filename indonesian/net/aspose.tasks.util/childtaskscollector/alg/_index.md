---
title: "ChildTasksCollector.Alg"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ChildTasksCollector. Memproses objek yang ditentukan"
type: docs
weight: 30
url: /id/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

Memproses objek yang ditentukan.

```csharp
public override void Alg(Task el, int level)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | Tugas | Objek untuk diproses. |
| tingkat | Int32 | Level node pohon. |

## Contoh

Menampilkan cara mengiterasi semua tugas dalam proyek sebagai daftar biasa.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Mengurai semua tugas yang dikumpulkan
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Lihat Juga

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


