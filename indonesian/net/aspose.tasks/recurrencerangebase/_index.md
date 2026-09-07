---
title: "Kelas RecurrenceRangeBase"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.RecurrenceRangeBase. Mewakili rentang berulang dari tugas berulang."
type: docs
weight: 1710
url: /id/net/aspose.tasks/recurrencerangebase/
---
## RecurrenceRangeBase class

Mewakili rentang pengulangan tugas berulang.

```csharp
public abstract class RecurrenceRangeBase
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Start](../../aspose.tasks/recurrencerangebase/start/) { get; set; } | Mendapatkan atau mengatur tanggal mulai rentang pengulangan tugas berulang. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


