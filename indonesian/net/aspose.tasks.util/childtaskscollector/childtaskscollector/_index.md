---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor ChildTasksCollector. Menginisialisasi sebuah instance baru dari kelas ChildTasksCollector"
type: docs
weight: 10
url: /id/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

Menginisialisasi sebuah instance baru dari kelas [`ChildTasksCollector`](../).

```csharp
public ChildTasksCollector()
```

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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


