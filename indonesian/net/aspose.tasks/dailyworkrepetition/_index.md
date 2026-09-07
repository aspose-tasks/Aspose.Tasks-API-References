---
title: "Kelas DailyWorkRepetition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.DailyWorkRepetition. Mewakili kelas untuk pengulangan dalam pola berulang harian berdasarkan hari kerja"
type: docs
weight: 420
url: /id/net/aspose.tasks/dailyworkrepetition/
---
## DailyWorkRepetition class

Mewakili kelas untuk pengulangan dalam pola berulang harian berdasarkan hari kerja.

```csharp
public class DailyWorkRepetition : DailyRepetitionBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [DailyWorkRepetition](dailyworkrepetition/)() | Menginisialisasi instance baru dari kelas `DailyWorkRepetition`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Mendapatkan atau mengatur jumlah hari yang mewakili interval dalam hari antara kejadian. |

## Contoh

Menampilkan cara bekerja dengan pengulangan pola kerja harian saat membuat tugas berulang.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "New recurrent task",
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     RecurrenceRange = new EndAfterRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 1, 1, 8, 0, 0), OccurrenceNumber = 9
                                                                           },
                                                     Repetition = new DailyWorkRepetition { RepetitionInterval = 1 }
                                                 },
                         Duration = project.GetDuration(1, TimeUnitType.Hour)
                     };
parameters.SetCalendar(project, "Standard");

var task = project.RootTask.Children.Add(parameters);
task.Set(Tsk.Start, new DateTime(2020, 4, 27, 8, 0, 0));

// lanjutkan bekerja dengan proyek...
// ...
```

### Lihat Juga

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


