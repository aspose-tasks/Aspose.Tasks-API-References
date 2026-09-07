---
title: "ChildTasksCollector.Tasks"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ChildTasksCollector. Mendapatkan daftar tugas objek anak yang dikumpulkan"
type: docs
weight: 20
url: /id/net/aspose.tasks.util/childtaskscollector/tasks/
---
## ChildTasksCollector.Tasks property

Mendapatkan daftar objek anak yang dikumpulkan (tugas).

```csharp
public List<Task> Tasks { get; }
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

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


