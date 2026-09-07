---
title: "TaskBaselineCollection.GetEnumerator"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "TaskBaselineCollection metode. Mengembalikan enumerator untuk koleksi ini"
type: docs
weight: 40
url: /id/net/aspose.tasks/taskbaselinecollection/getenumerator/
---
## TaskBaselineCollection.GetEnumerator method

Mengembalikan enumerator untuk koleksi ini.

```csharp
public IEnumerator<TaskBaseline> GetEnumerator()
```

### Nilai Kembali

enumerator untuk koleksi ini.

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

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


