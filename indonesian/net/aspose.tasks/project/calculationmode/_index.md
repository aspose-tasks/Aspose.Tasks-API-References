---
title: "Project.CalculationMode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan atau mengatur mode perhitungan sebuah proyek. Dapat menjadi salah satu nilai dari enumerasi CalculationMode"
type: docs
weight: 110
url: /id/net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

Mendapatkan atau mengatur mode perhitungan sebuah proyek. Dapat menjadi salah satu nilai dari enumerasi `CalculationMode`.

```csharp
public CalculationMode CalculationMode { get; set; }
```

## Contoh

Menampilkan cara menggunakan mode perhitungan proyek.

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

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


