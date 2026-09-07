---
title: "Duration.Convert"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Duration. Mengonversi objek Duration ke durasi lain dengan satuan waktu yang ditentukan"
type: docs
weight: 70
url: /id/net/aspose.tasks/duration/convert/
---
## Duration.Convert method

Mengonversi objek Duration ke durasi lain dengan unit waktu yang ditentukan.

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| timeUnitType | TimeUnitType | tipe satuan waktu yang ditentukan. |

### Nilai Kembali

mengembalikan durasi baru dengan tipe satuan yang ditentukan.

## Contoh

Menampilkan cara mengonversi durasi ke dalam berbagai tipe unit waktu.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Dapatkan tugas untuk menghitung durasinya dalam berbagai format
var task = project.RootTask.Children.GetById(1);

// Dapatkan durasi dalam Menit, Hari, Jam, Minggu, dan Bulan
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Lihat Juga

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


