---
title: "Enum CalculationMode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.CalculationMode enum. Menentukan mode perhitungan proyek"
type: docs
weight: 210
url: /id/net/aspose.tasks/calculationmode/
---
## CalculationMode enumeration

Menentukan mode perhitungan proyek.

```csharp
public enum CalculationMode
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| None | `0` | Tidak ada. Tanggal dan biaya proyek tidak dihitung ulang dalam mode ini. |
| Automatic | `1` | Mode otomatis. Tanggal dan biaya proyek dihitung ulang saat menggunakan mode ini. |
| Manual | `2` | Mode manual. Hanya bidang yang diperlukan yang dihitung ulang dalam mode ini, misalnya UID dan ID objek. |

## Contoh

Menampilkan cara menggunakan mode perhitungan otomatis.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Automatic
};

// Atur tanggal mulai proyek dan tambahkan tugas baru
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Tautkan tugas
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Verifikasi tanggal telah dihitung ulang
Console.WriteLine("Task1 Start + 1 Equals Task2 Start : {0} ", task1.Get(Tsk.Start).AddDays(1).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish + 1 Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).AddDays(1).Equals(task2.Get(Tsk.Finish)));
Console.WriteLine("RootTask Finish Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.RootTask.Get(Tsk.Finish)));
Console.WriteLine("Project Finish Date Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.Get(Prj.FinishDate)));
```

Menampilkan cara menggunakan mode perhitungan none.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

// Tambahkan tugas baru
var task = project.RootTask.Children.Add("Task");

// Catatan bahwa bahkan ID tidak dihitung            
Console.WriteLine("Task.Id Equals 0 : {0} ", task.Get(Tsk.Id).Equals(0));
Console.WriteLine("Task.OutlineLevel Equals 0 : {0} ", task.Get(Tsk.OutlineLevel).Equals(0));
Console.WriteLine("Task Start Equals DateTime.MinValue : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
Console.WriteLine("Task Duration Equals 0 mins : {0} ", task.Get(Tsk.Duration).ToString().Equals("0 mins"));

// Atur properti durasi
task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));
Console.WriteLine("Task Duration Equals 2 days : {0} ", task.Get(Tsk.Duration).ToString().Equals("2 days"));
Console.WriteLine("Task Start Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
```

Menampilkan cara menggunakan mode perhitungan manual.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// Atur tanggal mulai proyek dan tambahkan tugas baru
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Properti yang diperlukan diatur dalam mode manual
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// Ketika kami menautkan dua tugas bersama, tanggal mereka tidak dihitung ulang dalam mode manual
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Mulai Tugas 2 tidak berubah
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


