---
title: "Kelas TaskBaselineCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TaskBaselineCollection. Menunjukkan kumpulan objek TaskBaseline."
type: docs
weight: 2380
url: /id/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

Menunjukkan kumpulan objek [`TaskBaseline`](../taskbaseline/).

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | Mengambil jumlah objek yang terdapat dalam objek TaskBaselineCollection ini. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | Mengembalikan elemen pada indeks yang ditentukan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | Ini adalah implementasi stub dari metode Add milik ICollection, yang hanya melempar NotSupportedException |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | Menghapus baseline dari koleksi ini. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | Mengonversi objek TaskBaselineCollection menjadi daftar objek [`TaskBaseline`](../taskbaseline/). |

## Contoh

Menampilkan cara bekerja dengan koleksi baseline tugas.

```csharp
var project = new Project();

// buat baseline proyek
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// cetak baseline tugas
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// mari hapus semua baseline
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### Lihat Juga

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


