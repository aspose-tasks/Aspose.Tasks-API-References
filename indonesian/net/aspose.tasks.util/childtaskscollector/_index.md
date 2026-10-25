---
title: "Kelas ChildTasksCollector"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Util.ChildTasksCollector. Mengumpulkan semua tugas anak"
type: docs
weight: 2690
url: /id/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

Mengumpulkan semua tugas anak.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | Menginisialisasi instance baru dari kelas `ChildTasksCollector`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | Mendapatkan daftar objek anak yang dikumpulkan (tugas). |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | Memproses objek yang ditentukan. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


