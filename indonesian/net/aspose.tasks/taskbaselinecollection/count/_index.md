---
title: "TaskBaselineCollection.Count"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TaskBaselineCollection. Mendapatkan jumlah objek yang terkandung dalam objek TaskBaselineCollection ini"
type: docs
weight: 10
url: /id/net/aspose.tasks/taskbaselinecollection/count/
---
## TaskBaselineCollection.Count property

Mengambil jumlah objek yang terdapat dalam objek TaskBaselineCollection ini.

```csharp
public int Count { get; }
```

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

* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


