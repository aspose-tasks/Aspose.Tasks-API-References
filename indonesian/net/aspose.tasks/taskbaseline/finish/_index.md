---
title: "TaskBaseline.Finish"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TaskBaseline. Mendapatkan atau mengatur tanggal selesai terjadwal dari tugas ketika baseline disimpan"
type: docs
weight: 40
url: /id/net/aspose.tasks/taskbaseline/finish/
---
## TaskBaseline.Finish property

Mendapatkan atau mengatur tanggal selesai terjadwal dari tugas ketika baseline disimpan.

```csharp
public DateTime Finish { get; set; }
```

## Contoh

Menampilkan cara mengakses informasi baseline.

```csharp
var project = new Project();

// Membuat TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Tampilkan durasi baseline tugas
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// nilai yang menunjukkan apakah ini adalah Baseline Interim
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// cetak data berfase waktu dari baseline tugas
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### Lihat Juga

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


