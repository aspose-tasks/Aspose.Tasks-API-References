---
title: "TaskBaseline.TimephasedData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TaskBaseline. Mendapatkan atau mengatur instance TimephasedDataCollection untuk objek ini. Data berfase waktu yang terkait dengan baseline tugas."
type: docs
weight: 80
url: /id/net/aspose.tasks/taskbaseline/timephaseddata/
---
## TaskBaseline.TimephasedData property

Mendapatkan atau mengatur sebuah instance TimephasedDataCollection untuk objek ini. Data berfase waktu yang terkait dengan baseline tugas.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
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

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


