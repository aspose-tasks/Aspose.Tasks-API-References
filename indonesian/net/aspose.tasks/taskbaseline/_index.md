---
title: "Kelas TaskBaseline"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.TaskBaseline class. Mewakili Baseline dari sebuah Tugas"
type: docs
weight: 2370
url: /id/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

Mewakili Baseline dari sebuah Tugas.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | Menginisialisasi sebuah instance baru dari kelas `TaskBaseline`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Mendapatkan atau mengatur nomor unik dari catatan data baseline. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Mendapatkan atau mengatur biaya yang dianggarkan untuk pekerjaan yang dilakukan oleh sumber daya untuk proyek hingga saat ini. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Mendapatkan atau mengatur biaya anggaran dari pekerjaan yang dijadwalkan untuk sebuah sumber daya. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Mendapatkan atau mengatur biaya proyeksi sumber daya ketika baseline disimpan. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | Mendapatkan atau mengatur durasi terjadwal dari tugas ketika baseline disimpan. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah durasi baseline tugas diperkirakan. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | Mendapatkan atau mengatur tanggal selesai terjadwal dari tugas ketika baseline disimpan. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | Mendapatkan atau mengatur biaya tetap dari tugas ketika baseline disimpan. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah ini adalah Baseline Interim. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | Mendapatkan atau mengatur tanggal mulai terjadwal dari tugas ketika baseline disimpan. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | Mendapatkan atau mengatur sebuah instance TimephasedDataCollection untuk objek ini. Data berfase waktu yang terkait dengan baseline tugas. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Mendapatkan atau mengatur pekerjaan yang ditugaskan ke sumber daya ketika baseline disimpan. Jumlah pekerjaan yang ditugaskan ke sumber daya ketika baseline disimpan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek `TaskBaseline` yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | Mengembalikan nilai kode hash untuk instance dari kelas `TaskBaseline`. |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


