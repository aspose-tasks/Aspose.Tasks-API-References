---
title: "Duration.TimeUnit"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Duration. Mendapatkan tipe unit waktu untuk objek ini. Tipe unit waktu dari instance Duration ini"
type: docs
weight: 50
url: /id/net/aspose.tasks/duration/timeunit/
---
## Duration.TimeUnit property

Mendapatkan tipe unit waktu untuk objek ini. Tipe unit waktu dari instance Duration ini.

```csharp
public TimeUnitType TimeUnit { get; }
```

## Contoh

Menampilkan cara memperbarui durasi tugas.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// dapatkan tugas
var task1 = project.RootTask.Children.GetById(1);

// perbarui durasi tugas
var duration1 = task1.Get(Tsk.Duration);

// tambahkan satu hari ke tugas 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// atur durasi baru ke tugas
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// dapatkan tugas lain
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// ubah durasi dengan menggunakan tipe unit waktu aktual
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// atur durasi baru ke tugas
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Lihat Juga

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


