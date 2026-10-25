---
title: "Kelas DailyRecurrencePattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.DailyRecurrencePattern. Mewakili sekumpulan parameter yang digunakan untuk membuat tugas berulang harian dalam sebuah proyek"
type: docs
weight: 400
url: /id/net/aspose.tasks/dailyrecurrencepattern/
---
## DailyRecurrencePattern class

Mewakili sekumpulan parameter yang digunakan untuk membuat tugas berulang harian dalam sebuah proyek.

```csharp
public class DailyRecurrencePattern : RecurrencePatternBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [DailyRecurrencePattern](dailyrecurrencepattern/)() | Menginisialisasi instance baru dari kelas `DailyRecurrencePattern`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [RecurrenceRange](../../aspose.tasks/recurrencepatternbase/recurrencerange/) { get; set; } | Mendapatkan atau mengatur rentang pengulangan. |
| [Repetition](../../aspose.tasks/dailyrecurrencepattern/repetition/) { get; set; } | Mendapatkan atau mengatur pola pengulangan dalam pola pengulangan harian. |

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

* class [RecurrencePatternBase](../recurrencepatternbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


