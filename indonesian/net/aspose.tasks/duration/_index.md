---
title: "Struct Duration"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Struct Aspose.Tasks.Duration. Mewakili durasi dalam sebuah proyek"
type: docs
weight: 470
url: /id/net/aspose.tasks/duration/
---
## Duration structure

Mewakili durasi dalam sebuah proyek.

```csharp
public struct Duration : IEquatable<Duration>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Mendapatkan nilai yang menunjukkan apakah satuan waktu telah berlalu. Bendera yang menentukan apakah instance Duration ini telah berlalu. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Mendapatkan nilai yang menunjukkan apakah satuan waktu diperkirakan. Bendera yang menentukan apakah instance Duration ini diperkirakan. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Mendapatkan instance [`TimeSpan`](./timespan/) dari objek Duration ini. Instance TimeSpan dari objek Duration ini. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Mendapatkan tipe unit waktu untuk objek ini. Tipe unit waktu dari instance Duration ini. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Mengonversi string yang ditentukan menjadi instance struct `Duration`. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Menambahkan nilai double yang ditentukan ke durasi ini. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Menambahkan durasi yang ditentukan ke durasi ini. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Mengonversi objek Duration ke durasi lain dengan unit waktu yang ditentukan. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Mengembalikan nilai kode hash untuk objek ini. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Mengurangi nilai double yang ditentukan dari instance durasi ini. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Mengurangi durasi yang ditentukan dari instance durasi ini. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Mengonversi objek Duration menjadi nilai Double. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Mengembalikan representasi string dari instance ini. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | Menganalisis string durasi dalam format "PT--H--M--S--". |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Kembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


