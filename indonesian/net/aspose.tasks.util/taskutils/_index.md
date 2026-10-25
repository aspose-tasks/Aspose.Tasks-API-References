---
title: "Kelas TaskUtils"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Util.TaskUtils. Kelas pembantu yang menyediakan operasi berguna dengan tugas"
type: docs
weight: 2770
url: /id/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

Kelas pembantu yang menyediakan operasi berguna dengan tugas.

```csharp
public static class TaskUtils
```

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | Menerapkan algoritma yang ditentukan ke setiap tugas dalam pohon. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | Membangun pohon tugas baru yang memenuhi kondisi. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | Menemukan tugas yang memenuhi kondisi dalam pohon tugas. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | Menghitung secara rekursif jumlah tugas anak dari sebuah tugas melalui semua tingkatan. |

## Contoh

Menunjukkan cara bekerja dengan algoritma pohon.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// mengumpulkan semua tugas proyek
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// bekerja dengan tugas seperti daftar biasa
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### Lihat Juga

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


